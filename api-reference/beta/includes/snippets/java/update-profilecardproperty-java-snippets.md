---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 60bbda3e15fcf804e9c9ce834ce1528703495385
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972116"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfileCardProperty profileCardProperty = new ProfileCardProperty();
LinkedList<ProfileCardAnnotation> annotationsList = new LinkedList<ProfileCardAnnotation>();
ProfileCardAnnotation annotations = new ProfileCardAnnotation();
LinkedList<DisplayNameLocalization> localizationsList = new LinkedList<DisplayNameLocalization>();
DisplayNameLocalization localizations = new DisplayNameLocalization();
localizations.languageTag = "no-NB";
localizations.displayName = "Kostnads Senter";
localizationsList.add(localizations);
annotations.localizations = localizationsList;
annotationsList.add(annotations);
profileCardProperty.annotations = annotationsList;

graphClient.organization("{organizationId}").settings().profileCardProperties("CustomAttribute1")
    .buildRequest()
    .patch(profileCardProperty);

```