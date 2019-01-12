---
title: educationOneRosterApiDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при использовании OneRoster API в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 681a3331aba7bc84ac80911c4be8076d104f8a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938148"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="ca8c0-103">educationOneRosterApiDataProvider ресурсов</span><span class="sxs-lookup"><span data-stu-id="ca8c0-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="ca8c0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca8c0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca8c0-106">Используется для настройки синхронизации профилей данных school при использовании [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="ca8c0-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="ca8c0-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ca8c0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca8c0-108">Properties</span></span>

| <span data-ttu-id="ca8c0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca8c0-109">Property</span></span> | <span data-ttu-id="ca8c0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca8c0-110">Type</span></span> | <span data-ttu-id="ca8c0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca8c0-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ca8c0-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="ca8c0-112">**connectionUrl**</span></span> | <span data-ttu-id="ca8c0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8c0-113">String</span></span> | <span data-ttu-id="ca8c0-114">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="ca8c0-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="ca8c0-115">**schoolsIds**</span></span> | <span data-ttu-id="ca8c0-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ca8c0-116">String collection</span></span> |  <span data-ttu-id="ca8c0-117">Список sourcedIds school для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="ca8c0-118">**providerName**</span><span class="sxs-lookup"><span data-stu-id="ca8c0-118">**providerName**</span></span> | <span data-ttu-id="ca8c0-119">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8c0-119">String</span></span> | <span data-ttu-id="ca8c0-120">Имя поставщика услуг OneRoster, определенный в [спецификации OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="ca8c0-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="ca8c0-121">**connectionsettings используется для определения**</span><span class="sxs-lookup"><span data-stu-id="ca8c0-121">**connectionSettings**</span></span> | [<span data-ttu-id="ca8c0-122">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="ca8c0-122">educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="ca8c0-123">Параметры подключения для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="ca8c0-124">Должен иметь тип [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ca8c0-124">Should be of type [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="ca8c0-125">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="ca8c0-125">**customizations**</span></span> | [<span data-ttu-id="ca8c0-126">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="ca8c0-126">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="ca8c0-127">Дополнительные настройки применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="ca8c0-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca8c0-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca8c0-128">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
