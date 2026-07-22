mport itertools
all_words = list(itertools.chain.from_iterable([[word for word, tag in sent] for sent in sentences]))
all_tags = list(itertools.chain.from_iterable([[tag for word, tag in sent] for sent in sentences]))
unique_words = sorted(list(set(all_words)))
unique_tags = sorted(list(set(all_tags)))
print(f"\nTotal unique words in Brown Corpus: {len(unique_words)}")
print(f"Sample unique words: {unique_words[:10]}...")
print(f"\nTotal unique POS tags in Brown Corpus: {len(unique_tags)}")
print(f"Unique POS tags: {unique_tags}")# mkeerthi_12
