-- আমার এলাকা
create table my_area (
  id uuid primary key default uuid_generate_v4(),
  title text,
  description text
);

-- জরুরি সেবা
create table emergency_services (
  id uuid primary key default uuid_generate_v4(),
  service_name text,
  location text,
  contact_number text
);

-- শিক্ষাবৃত্তি
create table scholarships (
  id uuid primary key default uuid_generate_v4(),
  name text,
  eligibility text,
  application_deadline date,
  apply_link text
);

-- চাকরি ও প্রশিক্ষণ
create table jobs_and_training (
  id uuid primary key default uuid_generate_v4(),
  title text,
  description text,
  deadline date,
  apply_link text
);

-- স্বাস্থ্য কেন্দ্র
create table health_centers (
  id uuid primary key default uuid_generate_v4(),
  name text,
  location text,
  contact text,
  service_type text
);

-- পুলিশ স্টেশন
create table police_stations (
  id uuid primary key default uuid_generate_v4(),
  name text,
  location text,
  officer_name text,
  contact_number text
);

-- আমার কার্যক্রম
create table my_activities (
  id uuid primary key default uuid_generate_v4(),
  title text,
  description text,
  media_url text,
  activity_date date
);
