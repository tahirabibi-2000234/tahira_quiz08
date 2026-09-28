 # step 1 Next.js folder
  cd tahira_next.js
## step2 Supabase.js
  npm install @supabase/supabase-js




### step3 .env.local
</> env
NEXT_PUBLIC_SUPABASE_URL=https://your-project-id,supabase.com
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=your-publishable-key

</>   upabase Dashboard:Project → Project Settings → API
Project URL → NEXT_PUBLIC_SUPABASE_URL=https:// abcxyz. supabase.com
Publishable key → NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=sb_publishable_xxxxxxxxx

#### step4
##### step5
import { createClient } from '@supabase/supabase-js';

export const supabase = createClient(
  process.env.NEXT_PUBLIC_SUPABASE_URL,
  process.env.NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY
);

 ###### step6 department table:
CREATE TABLE department (
  department_id INT PRIMARY KEY,
  department_name VARCHAR(100) NOT NULL,
  location VARCHAR(100)
);

 ###### step INSERT INTO department
INSERT INTO department
 (department_id, department_name, location)
VALUES
(1, 'IT', 'Karachi'),
(2, 'HR', 'Lahore'),
(3, 'Finance', 'Islamabad');