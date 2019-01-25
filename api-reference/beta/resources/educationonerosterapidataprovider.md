---
title: educationOneRosterApiDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при использовании OneRoster API в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527985"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="20197-103">educationOneRosterApiDataProvider ресурсов</span><span class="sxs-lookup"><span data-stu-id="20197-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20197-104">Используется для настройки синхронизации профилей данных school при использовании [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="20197-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="20197-105">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="20197-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20197-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="20197-106">Properties</span></span>

| <span data-ttu-id="20197-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="20197-107">Property</span></span> | <span data-ttu-id="20197-108">Тип</span><span class="sxs-lookup"><span data-stu-id="20197-108">Type</span></span> | <span data-ttu-id="20197-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20197-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="20197-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="20197-110">**connectionUrl**</span></span> | <span data-ttu-id="20197-111">String</span><span class="sxs-lookup"><span data-stu-id="20197-111">String</span></span> | <span data-ttu-id="20197-112">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="20197-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="20197-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="20197-113">**schoolsIds**</span></span> | <span data-ttu-id="20197-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="20197-114">String collection</span></span> |  <span data-ttu-id="20197-115">Список sourcedIds school для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="20197-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="20197-116">ProviderName</span><span class="sxs-lookup"><span data-stu-id="20197-116">**providerName**</span></span> | <span data-ttu-id="20197-117">String</span><span class="sxs-lookup"><span data-stu-id="20197-117">String</span></span> | <span data-ttu-id="20197-118">Имя поставщика услуг OneRoster, определенный в [спецификации OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="20197-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="20197-119">**connectionsettings используется для определения**</span><span class="sxs-lookup"><span data-stu-id="20197-119">**connectionSettings**</span></span> | [<span data-ttu-id="20197-120">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="20197-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="20197-121">Параметры подключения для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="20197-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="20197-122">Должен иметь тип [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="20197-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="20197-123">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="20197-123">**customizations**</span></span> | [<span data-ttu-id="20197-124">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="20197-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="20197-125">Дополнительные настройки применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="20197-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20197-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20197-126">JSON representation</span></span>
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
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
