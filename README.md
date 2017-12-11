# Suicide Notes
A collection of people's suicide notes. This is a companion to my other project, ["Their Last Words."](https://github.com/CodeWritingCow/their-last-words)


## Contribute
Making a contribution is easy:
- Fork the repo.
- Add a JSON file with the person's suicide note and brief biography. See specs below.
- Check other pull requests to make sure you aren't submitting duplicates.
- Make a pull request.


## Specs
### File Name
Each person's suicide note is stored in a JSON file inside `collection/`. Name the JSON file like this:

**`collection/{lastname-firstname}.json:`**

If the person has a middle name, then name the file like this: **`{lastname-firstname-middlename}.json:`**

### File Structure
Use this structure for the JSON file.

```js
{
	"lastName": "",
	"firstName": "", // If person has a middle name, include it here
	"suicideNote": "",
	"translation": "", // If suicide note is in a non-English language, include English translation
	"biography": "", // One-sentence biography
	"born": "", // YYYY-MM-DD or YYYY. If date is unknown, omit this.
	"died": "", // YYYY-MM-DD or YYYT. See note above.
	"suicideMethod": "" // Suicide method
}
```
If the person's last words were in English, **`translation`** can be omitted from the file.

Note: Please remove comments from your JSON files. JSON doesn't allow comments. The comments in the template above are for illustrative purposes only.

## Example 
**`collections/cheung-leslie.json`**

```js
{
	"lastName": "Cheung",
	"firstName": "Leslie",
	"suicideNote": "Depression!! 多謝各位朋友，多謝麥列菲菲教授。 一年來很辛苦，不能再忍受，多謝唐先生，多謝家人，多謝肥姐。 我一生冇做壞事，為何這樣？？？ - Leslie",
	"translation": "Depression! Many thanks to all my friends. Many thanks to Professor Felice Lieh-Mak. This year has been so tough. I can't stand it anymore. Many thanks to Mr. Tong. Many thanks to my family. Many thanks to Sister Fei. In my life I have done nothing bad. Why does it have to be like this?",
	"biography": "Hong Kong singer and actor",
	"born": "1956-09-12",
	"died": "2003-04-01",
	"suicideMethod": "Jumped off building"
}
```
