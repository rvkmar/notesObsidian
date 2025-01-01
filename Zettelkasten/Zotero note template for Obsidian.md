
# Note template to be updated in Zotero program
```

{{if color == '#ff6666'}}
	<h2>{{highlight quotes='false'}}</h2>
{{elseif color == '#2ea8e5'}}
	{{if comment}}<p>{{comment}}:</p>{{endif}}<blockquote>{{highlight}}</blockquote><p>{{citation}}</p>
{{else}}
	<p>{{highlight}} {{citation}} {{comment}}{{if tags}} #{{tags join=' #'}}{{endif}}</p>
{{endif}}



new
{{if color == '#aaaaaa'}}
	<p>⬛ [[Argument]]: {{if comment}}<p>{{comment}}:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}</p>
{{else}}
	<p>{{highlight}} {{citation}} {{comment}}{{if tags}} #{{tags join=' #'}}{{endif}}</p>
{{endif}}



old
<p>{{highlight}} {{citation}} {{comment}}</p>
old
{{if color == '#aaaaaa'}} 	<p><span>[[Argument]]:: </span>{{highlight quotes='false'}} {{comment}} {{citation}}</p> {{else}} 	<p>{{highlight}} {{citation}} {{comment}}{{if tags}} #{{tags join=' #'}}{{endif}}</p> {{endif}}

----
"Gray": "[[Argument]]:", "Red": "[[Disagreement]]:", "Orange": "[[Critique]]", "Yellow": "", "Green": "- [ ] #litreview", "Cyan": "[[Field]]", "Blue": "[[Confusion]]:", "Magenta": "[[Useful for Research]]:"}
----

"Gray": "[[Argument]]:", "Red": "[[Disagreement]]:", "Orange": "[[Idea]]", "Yellow": "", "Green": "- [ ] ", "Cyan": "[[Important]]", "Blue": "[[Confusion]]:", "Magenta": "[[Critique]]:"}

yellow: '#ffd400', 
red: '#ff6666', 	[[Disagreement]]:
green: '#5fb236',	- [ ]  		#litreview
blue: '#2ea8e5', 	[[Confusion]]:	
purple: '#a28ae5', 
magenta: '#e56eee', 	[[Critique]]:	[[Useful for Research]]:	
orange: '#f19837',	[[Idea]] 	[[Critique]]
gray: '#aaaaaa'		[[Argument]]:

missing
"Cyan": "[[Important]]" 	"Cyan": "[[Field]]"

Notetemplate.title 
old
<h1>{{title}}<br/>({{date}})</h1>
new
<h1>{{title}}</h1>

noteTemplate highlight
{{if color == '#ffd400'}}
	<p> <span style="color:#ffd400;">💡 [[Idea]] 🤔 {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{elseif color == '#ff6666'}}
	<p> <span style="color:#ff6666;">🔴 [[Disagreement]] 💔  {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{elseif color == '#5fb236'}}
	<p> <span style="color:#5fb236;">🟢 [[Important]] 🎁  {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{elseif color == '#2ea8e5'}}
	<p> <span style="color:#2ea8e5;">🔵 [[Argument]] 🔥  {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{elseif color == '#a28ae5'}}
	<p> <span style="color:#a28ae5;">🟣 [[Critique]] ‼️  {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{elseif color == '#e56eee'}}
	<p> <span style="color:#e56eee;">🔷 [[Confusion]] 😵‍💫  {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{elseif color == '#f19837'}}
	<p> <span style="color:#f19837;">🟠 [[Todo]] 📝  {{if comment}}<p>_{{comment}}_:</p>{{endif}} <p> - [ ]  {{highlight quotes='false'}} <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}}
{{else}}
	<p>{{highlight}} {{citation}} {{comment}}{{if tags}} #{{tags join=' #'}}{{endif}}</p>
{{endif}}


Annotation Color Guide:

💡 Yellow: Idea
🔴 Red: Disagreement
🟢 Green: Important
🔵 Blue: Argument
🟣 Purple: Critique
🔷 Magenta: Confusion
🟠 Orange: Todo
🔲 Gray: Miscellaneous


---
{{if color == '#ffd400'}}
	<h4> 💡 Idea 🤔 </h4> <p> [[Idea]] {{if comment}} <p> *Comment:* {{comment}}</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{elseif color == '#ff6666'}}
	<h4> 🔴 Disagreement 💔 </h4> <p> [[Disagreement]] {{if comment}}<p> *Comment:* {{comment}}</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{elseif color == '#5fb236'}}
	<h4> 🟢 Important 🎁 </h4> <p> [[Important]]  {{if comment}}<p> *Comment:* {{comment}}</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{elseif color == '#2ea8e5'}}
	<h4> 🔵 Argument 🔥 </h4> <p> [[Argument]]  {{if comment}}<p> *Comment:* {{comment}}</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{elseif color == '#a28ae5'}}
	<h4> 🟣 Critique ‼️ </h4> <p> [[Critique]]  {{if comment}}<p> *Comment:* {{comment}}</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{elseif color == '#e56eee'}}
	<h4> 🔷 Confusion 😵‍💫  </h4> <p> [[Confusion]]  {{if comment}}<p> *Comment:* {{comment}}</p>{{endif}} <p> > [!quote] > {{highlight quotes='false'}} <br> <span style="color:GoldenRod;">{{citation}} </span> </p> {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{elseif color == '#f19837'}}
	<h4> 🟠 Todo 📝 </h4> <p> - [ ]  {{highlight quotes='false'}} <span style="color:GoldenRod;">{{citation}} </span> {{if comment}}<p> Comment: _{{comment}}_</p>{{endif}} {{if tags}} #{{tags join=' #'}} {{endif}} </p>
{{else}}
	<p>{{highlight}} {{citation}} <br> Comment: _{{comment}}_ {{if tags}} #{{tags join=' #'}}{{endif}}</p>
{{endif}}

---
```