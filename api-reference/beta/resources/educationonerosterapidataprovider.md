---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ea02186b7d9bd7bed14c6ea5b46023da81814f07
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791064"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="dbefd-103">ресурс Едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="dbefd-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="dbefd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbefd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbefd-105">Используется для настройки профиля синхронизации данных School при использовании [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="dbefd-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="dbefd-106">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="dbefd-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dbefd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbefd-107">Properties</span></span>

| <span data-ttu-id="dbefd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbefd-108">Property</span></span>           | <span data-ttu-id="dbefd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dbefd-109">Type</span></span>                                         | <span data-ttu-id="dbefd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dbefd-110">Description</span></span>                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="dbefd-111">коннектионурл</span><span class="sxs-lookup"><span data-stu-id="dbefd-111">connectionUrl</span></span>      | <span data-ttu-id="dbefd-112">String</span><span class="sxs-lookup"><span data-stu-id="dbefd-112">String</span></span>                                       | <span data-ttu-id="dbefd-113">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="dbefd-113">The connection URL to the OneRoster instance.</span></span>                                                         |
| <span data-ttu-id="dbefd-114">providerName</span><span class="sxs-lookup"><span data-stu-id="dbefd-114">providerName</span></span>       | <span data-ttu-id="dbefd-115">String</span><span class="sxs-lookup"><span data-stu-id="dbefd-115">String</span></span>                                       | <span data-ttu-id="dbefd-116">Имя поставщика службы OneRoster, как определено [спецификацией OneRoster][oneroster].</span><span class="sxs-lookup"><span data-stu-id="dbefd-116">The OneRoster Service Provider name as defined by the [OneRoster specification][oneroster].</span></span>           |
| <span data-ttu-id="dbefd-117">счулсидс</span><span class="sxs-lookup"><span data-stu-id="dbefd-117">schoolsIds</span></span>         | <span data-ttu-id="dbefd-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dbefd-118">String collection</span></span>                            | <span data-ttu-id="dbefd-119">Список учебных заведений [или организации][orgs] `sourcedId` для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dbefd-119">The list of [School/Org][orgs] `sourcedId` to sync.</span></span>                                                   |
| <span data-ttu-id="dbefd-120">термидс</span><span class="sxs-lookup"><span data-stu-id="dbefd-120">termIds</span></span>            | <span data-ttu-id="dbefd-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dbefd-121">String collection</span></span>                            | <span data-ttu-id="dbefd-122">Список [учебных лекций][terms] для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dbefd-122">The list of [academic sessions][terms] to sync.</span></span>                                                       |
| <span data-ttu-id="dbefd-123">коннектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="dbefd-123">connectionSettings</span></span> | <span data-ttu-id="dbefd-124">[едукатионсинчронизатионконнектионсеттингс]</span><span class="sxs-lookup"><span data-stu-id="dbefd-124">[educationSynchronizationConnectionSettings]</span></span> | <span data-ttu-id="dbefd-125">Параметры [oauth 1,0][onerosteroauth1] или [OAuth 2,0][onerosteroauth2] для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="dbefd-125">The [OAuth 1.0][onerosteroauth1] or [OAuth 2.0][onerosteroauth2] settings for the OneRoster instance.</span></span> |
| <span data-ttu-id="dbefd-126">настроек</span><span class="sxs-lookup"><span data-stu-id="dbefd-126">customizations</span></span>     | <span data-ttu-id="dbefd-127">[едукатионсинчронизатионкустомизатионс])</span><span class="sxs-lookup"><span data-stu-id="dbefd-127">[educationSynchronizationCustomizations])</span></span>    | <span data-ttu-id="dbefd-128">Необязательная настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dbefd-128">Optional customization to be applied to the synchronization profile.</span></span>                                  |

> [!IMPORTANT]
> <span data-ttu-id="dbefd-129">В OneRoster для сегментирования данных используются учебные сеансы, а не один учебный год.</span><span class="sxs-lookup"><span data-stu-id="dbefd-129">OneRoster uses academic sessions rather than a single school year to segment their data.</span></span> <span data-ttu-id="dbefd-130">Эта сегментация абстрактна в пользовательском интерфейсе "School Data Sync", но не является этим API.</span><span class="sxs-lookup"><span data-stu-id="dbefd-130">This segmentation is abstracted away within School Data Sync UI but not this API.</span></span> <span data-ttu-id="dbefd-131">Для заполнения коллекции необходимо вызвать `/terms` конечную точку OneRoster для получения коллекции академических идентификаторов сеансов `termIds` .</span><span class="sxs-lookup"><span data-stu-id="dbefd-131">You will need to call the OneRoster `/terms` endpoint to get the collection of academic session IDs in order to populate the `termIds` collection.</span></span>

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md
[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[едукатионсинчронизатионкустомизатионс]: educationsynchronizationcustomizations.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a><span data-ttu-id="dbefd-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbefd-134">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->
