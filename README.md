- 0x2char.py — Replaces each (MySQL) 0x<hex> encoded string with equivalent CONCAT(CHAR(),…) counterpart
  
 - apostrophemask.py — Replaces apostrophe character (‘) with its UTF-8 full width counterpart (e.g. ‘ -> %EF%BC%87)
 
 - apostrophenullencode.py — Replaces apostrophe character (‘) with its illegal double unicode counterpart (e.g. ‘ -> %00%27)
 
 - appendnullbyte.py — Appends (Access) NULL byte character (%00) at the end of payload
 
 - base64encode.py — Base64-encodes all characters in a given payload
 
 - between.py — Replaces greater than operator (‘>’) with ‘NOT BETWEEN 0 AND #’ and equals operator (‘=’) with ‘BETWEEN # AND #’
 
 - bluecoat.py — Replaces space character after SQL statement with a valid random blank character. Afterwards replace character ‘=’ with operator LIKE
 
 - chardoubleencode.py — Double URL-encodes all characters in a given payload (not processing already encoded) (e.g. SELECT -> %2553%2545%254C%2545%2543%2554)
 
 - charencode.py — URL-encodes all characters in a given payload (not processing already encoded) (e.g. SELECT -> %53%45%4C%45%43%54)
 
 - charunicodeencode.py — Unicode-URL-encodes all characters in a given payload (not processing already encoded) (e.g. SELECT -> %u0053%u0045%u004C%u0045%u0043%u0054)
 
 - charunicodeescape.py — Unicode-escapes non-encoded characters in a given payload (not processing already encoded) (e.g. SELECT -> \u0053\u0045\u004C\u0045\u0043\u0054)
 
 
 - commalesslimit.py — Replaces (MySQL) instances like ‘LIMIT M, N’ with ‘LIMIT N OFFSET M’ counterpart
 
 
 
 - commalessmid.py — Replaces (MySQL) instances like ‘MID(A, B, C)’ with ‘MID(A FROM B FOR C)’ counterpart
 - commentbeforeparentheses.py — Prepends (inline) comment before parentheses (e.g. ( -> /**/()
 - concat2concatws.py — Replaces (MySQL) instances like ‘CONCAT(A, B)’ with ‘CONCAT_WS(MID(CHAR(0), 0, 0), A, B)’ counterpart
 - equaltolike.py — Replaces all occurrences of operator equal (‘=’) with ‘LIKE’ counterpart
 - escapequotes.py — Slash escape single and double quotes (e.g. ‘ -> \’)
 - greatest.py — Replaces greater than operator (‘>’) with ‘GREATEST’ counterpart
 - halfversionedmorekeywords.py — Adds (MySQL) versioned comment before each keyword
 - htmlencode.py — HTML encode (using code points) all non-alphanumeric characters (e.g. ‘ -> &#39;)
 - ifnull2casewhenisnull.py — Replaces instances like ‘IFNULL(A, B)’ with ‘CASE WHEN ISNULL(A) THEN (B) ELSE (A) END’ counterpart
 - ifnull2ifisnull.py — Replaces instances like ‘IFNULL(A, B)’ with ‘IF(ISNULL(A), B, A)’ counterpart
 - informationschemacomment.py — Add an inline comment (/**/) to the end of all occurrences of (MySQL) “information_schema” identifier
 - least.py — Replaces greater than operator (‘>’) with ‘LEAST’ counterpart
 - lowercase.py — Replaces each keyword character with lower case value (e.g. SELECT -> select)
 - luanginx.py — LUA-Nginx WAFs Bypass (e.g. Cloudflare)
 - modsecurityversioned.py — Embraces complete query with (MySQL) versioned comment
 - modsecurityzeroversioned.py — Embraces complete query with (MySQL) zero-versioned comment
 - multiplespaces.py — Adds multiple spaces (‘ ‘) around SQL keywords
 - overlongutf8.py — Converts all (non-alphanum) characters in a given payload to overlong UTF8 (not processing already encoded) (e.g. ‘ -> %C0%A7)
 - overlongutf8more.py — Converts all characters in a given payload to overlong UTF8 (not processing already encoded) (e.g. SELECT -> %C1%93%C1%85%C1%8C%C1%85%C1%83%C1%94)
 - percentage.py — Adds a percentage sign (‘%’) infront of each character (e.g. SELECT -> %S%E%L%E%C%T)
 - plus2concat.py — Replaces plus operator (‘+’) with (MsSQL) function CONCAT() counterpart
 - plus2fnconcat.py — Replaces plus operator (‘+’) with (MsSQL) ODBC function {fn CONCAT()} counterpart
 - randomcase.py — Replaces each keyword character with random case value (e.g. SELECT -> SEleCt)
 - randomcomments.py — Add random inline comments inside SQL keywrds (e.g. SELECT -> S/** /E/* */LECT)
