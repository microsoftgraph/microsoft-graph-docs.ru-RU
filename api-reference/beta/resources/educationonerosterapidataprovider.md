---
title: ресурс educationOneRosterApiDataProvider
description: Используется для настройка профиля синхронизации школьных данных, когда API OneRoster используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2c90c7132f6e51b84e987cf6bda63baacc60b8ba
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080423"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="087ba-103">ресурс educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="087ba-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="087ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="087ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="087ba-105">Используется для настройка профиля синхронизации школьных данных, когда [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) используется в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="087ba-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="087ba-106">Производный от [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="087ba-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="087ba-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="087ba-107">Properties</span></span>

| <span data-ttu-id="087ba-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="087ba-108">Property</span></span>           | <span data-ttu-id="087ba-109">Тип</span><span class="sxs-lookup"><span data-stu-id="087ba-109">Type</span></span>                                         | <span data-ttu-id="087ba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="087ba-110">Description</span></span>                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="087ba-111">connectionUrl</span><span class="sxs-lookup"><span data-stu-id="087ba-111">connectionUrl</span></span>      | <span data-ttu-id="087ba-112">String</span><span class="sxs-lookup"><span data-stu-id="087ba-112">String</span></span>                                       | <span data-ttu-id="087ba-113">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="087ba-113">The connection URL to the OneRoster instance.</span></span>                                                         |
| <span data-ttu-id="087ba-114">providerName</span><span class="sxs-lookup"><span data-stu-id="087ba-114">providerName</span></span>       | <span data-ttu-id="087ba-115">String</span><span class="sxs-lookup"><span data-stu-id="087ba-115">String</span></span>                                       | <span data-ttu-id="087ba-116">Имя поставщика услуг OneRoster, определенное спецификацией [OneRoster.][oneroster]</span><span class="sxs-lookup"><span data-stu-id="087ba-116">The OneRoster Service Provider name as defined by the [OneRoster specification][oneroster].</span></span>           |
| <span data-ttu-id="087ba-117">schoolsIds</span><span class="sxs-lookup"><span data-stu-id="087ba-117">schoolsIds</span></span>         | <span data-ttu-id="087ba-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="087ba-118">String collection</span></span>                            | <span data-ttu-id="087ba-119">Список [синхронизируются с School/Org.][orgs] `sourcedId`</span><span class="sxs-lookup"><span data-stu-id="087ba-119">The list of [School/Org][orgs] `sourcedId` to sync.</span></span>                                                   |
| <span data-ttu-id="087ba-120">termIds</span><span class="sxs-lookup"><span data-stu-id="087ba-120">termIds</span></span>            | <span data-ttu-id="087ba-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="087ba-121">String collection</span></span>                            | <span data-ttu-id="087ba-122">Список [академических сеансов для][terms] синхронизации.</span><span class="sxs-lookup"><span data-stu-id="087ba-122">The list of [academic sessions][terms] to sync.</span></span>                                                       |
| <span data-ttu-id="087ba-123">connectionSettings</span><span class="sxs-lookup"><span data-stu-id="087ba-123">connectionSettings</span></span> | <span data-ttu-id="087ba-124">[educationSynchronizationConnectionSettings]</span><span class="sxs-lookup"><span data-stu-id="087ba-124">[educationSynchronizationConnectionSettings]</span></span> | <span data-ttu-id="087ba-125">Параметры [OAuth 1.0][onerosteroauth1] или [OAuth 2.0][onerosteroauth2] для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="087ba-125">The [OAuth 1.0][onerosteroauth1] or [OAuth 2.0][onerosteroauth2] settings for the OneRoster instance.</span></span> |
| <span data-ttu-id="087ba-126">настройки</span><span class="sxs-lookup"><span data-stu-id="087ba-126">customizations</span></span>     | <span data-ttu-id="087ba-127">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="087ba-127">[educationSynchronizationCustomizations]</span></span>    | <span data-ttu-id="087ba-128">Необязательная настройка, которая будет применена к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="087ba-128">Optional customization to be applied to the synchronization profile.</span></span>                                  |

> [!IMPORTANT]
> <span data-ttu-id="087ba-129">OneRoster использует академические сеансы, а не один учебный год для сегментации данных.</span><span class="sxs-lookup"><span data-stu-id="087ba-129">OneRoster uses academic sessions rather than a single school year to segment their data.</span></span> <span data-ttu-id="087ba-130">Эта сегментация абстрагироваться в Синхронизация сведений о школе пользовательского интерфейса, но не этот API.</span><span class="sxs-lookup"><span data-stu-id="087ba-130">This segmentation is abstracted away within School Data Sync UI but not this API.</span></span> <span data-ttu-id="087ba-131">Чтобы заполнить коллекцию, необходимо вызвать конечную точку OneRoster, чтобы получить коллекцию академических ИД `/terms` `termIds` сеансов.</span><span class="sxs-lookup"><span data-stu-id="087ba-131">You will need to call the OneRoster `/terms` endpoint to get the collection of academic session IDs in order to populate the `termIds` collection.</span></span>

[educationSynchronizationConnectionSettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a><span data-ttu-id="087ba-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="087ba-134">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
    "clientId": "String",
    "clientSecret&quot;: &quot;String"
  },
  "customizations": {
    "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
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
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.ediscovery.settings"
  ]
}-->


