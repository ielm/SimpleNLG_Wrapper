## SimpleNLG Features

The features package contains enumerated types that are used for
specific features. A complete list of currently implemented features is
given in the abstract class {@code Feature}. Particular attention should
be paid to using the correct type with these features and, when
introducing new features, that existing feature names are not
overwritten.
Features are stored as a Map; String, Object;
on the NLGElement. The base way of accessing features is
through the getFeature() and setFeature()
methods. There are additional convenience methods for converting the
feature object to a particular type. In addition, classes extending from
NLGElement may have additional convenience methods for
accessing features.

The contents of this file are subject to the Mozilla Public
License Version 1.1 (the "License"); you may not use this file except in
compliance with the License. You may obtain a copy of the License at
http://www.mozilla.org/MPL/

Software distributed under the License is distributed on an "AS
IS" basis, WITHOUT WARRANTY OF ANY KIND, either express or implied. See
the License for the specific language governing rights and limitations
under the License.

The Original Code is "Simplenlg".

The Initial Developer of the Original Code is Ehud Reiter, Albert
Gatt and Dave Westwater. Portions created by Ehud Reiter, Albert Gatt
and Dave Westwater are Copyright (C) 2010-11 The University of Aberdeen.
All Rights Reserved.

Contributor(s): Ehud Reiter, Albert Gatt, Dave Wewstwater, Roman
Kutlak, Margaret Mitchell.