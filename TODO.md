
sudo apk add gmp-dev git-lfs

stack install hoogle-5.0.18.4
stack install ghcid-0.8.9
stack install hlint-3.6.1
stack install cabal-fmt-0.1.11
stack install cabal-gild-1.5.0.1
stack install fourmolu-0.14.0.0

echo >> ~/.ghci ':def hoogle \x -> return $ ":!hoogle \"" ++ x ++ "\""'
echo >> ~/.ghci ':def rmain  \x -> return ":reload\n:main"'

ghcid -T main -c "stack repl Set1Test.hs"

https://github.com/i-tu/Hasklig/releases/download/v1.2/Hasklig-1.2.zip
