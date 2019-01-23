---
title: educationOneRosterApiDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при использовании OneRoster API в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ccfb74cdac64a147adb8ed7d3a0ad4b3fa3c83cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425990"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="64d22-103">educationOneRosterApiDataProvider ресурсов</span><span class="sxs-lookup"><span data-stu-id="64d22-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="64d22-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64d22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64d22-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64d22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64d22-106">Используется для настройки синхронизации профилей данных school при использовании [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="64d22-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="64d22-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="64d22-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="64d22-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64d22-108">Properties</span></span>

| <span data-ttu-id="64d22-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64d22-109">Property</span></span> | <span data-ttu-id="64d22-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64d22-110">Type</span></span> | <span data-ttu-id="64d22-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64d22-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="64d22-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="64d22-112">**connectionUrl**</span></span> | <span data-ttu-id="64d22-113">String</span><span class="sxs-lookup"><span data-stu-id="64d22-113">String</span></span> | <span data-ttu-id="64d22-114">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="64d22-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="64d22-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="64d22-115">**schoolsIds**</span></span> | <span data-ttu-id="64d22-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64d22-116">String collection</span></span> |  <span data-ttu-id="64d22-117">Список sourcedIds school для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="64d22-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="64d22-118">**providerName**</span><span class="sxs-lookup"><span data-stu-id="64d22-118">**providerName**</span></span> | <span data-ttu-id="64d22-119">String</span><span class="sxs-lookup"><span data-stu-id="64d22-119">String</span></span> | <span data-ttu-id="64d22-120">Имя поставщика услуг OneRoster, определенный в [спецификации OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="64d22-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="64d22-121">**connectionsettings используется для определения**</span><span class="sxs-lookup"><span data-stu-id="64d22-121">**connectionSettings**</span></span> | [<span data-ttu-id="64d22-122">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="64d22-122">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="64d22-123">Параметры подключения для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="64d22-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="64d22-124">Должен иметь тип [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="64d22-124">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="64d22-125">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="64d22-125">**customizations**</span></span> | [<span data-ttu-id="64d22-126">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="64d22-126">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="64d22-127">Дополнительные настройки применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="64d22-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64d22-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64d22-128">JSON representation</span></span>
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
