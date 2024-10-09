# Wtf site

> various link

- https://motherfuckingwebsite.com/
- http://madebyevan.com/webgl-water/
- https://github.com/yurkagon/Doom-Nukem-CSS
- https://paveldogreat.github.io/-
- WebGL-Fluid-Simulation/
- https://codepen.io/amit_sheen/pen/QWGjRKR
- https://codepen.io/RTarson/pen/yvyvmq

# Command
> command
```sh
replace GIT_LAB_URL wit hyour gitlab url
replace YOUR_TOKEN with your gitlab token
for id in $(curl -s --header "PRIVATE-TOKEN: YOUR_TOKEN" https://GIT_LAB_URL/api/v4/groups/ | jq -r '.[].id'); do for repo in $(curl -s --header "PRIVATE-TOKEN: YOUR_TOKEN" https://GIT_LAB_URL/api/v4/groups/$id| jq -r ".projects[].ssh_url_to_repo"); do git clone $repo; done; done;
# remove some files
find . '(' -name "node_modules" -o -name "__pycache__" -o -name ".git" -o -name "*.tar.gz" ')'
```
