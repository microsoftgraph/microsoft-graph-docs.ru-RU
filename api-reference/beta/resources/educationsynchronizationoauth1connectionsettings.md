---
title: educationSynchronizationOAuth1ConnectionSettings ресурсов
description: При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 80921488e1a5e0dd3e4ab4e21b2ea08e05ad9cee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990266"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="a6b40-103">educationSynchronizationOAuth1ConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="a6b40-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="a6b40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6b40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6b40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6b40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6b40-106">При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="a6b40-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="a6b40-107">На основе [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a6b40-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a6b40-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6b40-108">Properties</span></span>

<span data-ttu-id="a6b40-109">Дополнительные свойства, предоставляемые интерфейсом этого типа.</span><span class="sxs-lookup"><span data-stu-id="a6b40-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6b40-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6b40-110">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
