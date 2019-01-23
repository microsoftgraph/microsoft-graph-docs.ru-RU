---
title: educationSynchronizationOAuth1ConnectionSettings ресурсов
description: При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2cc8a0fee08826fef7d560a18f730bd7d58a2f6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417233"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="c1c02-103">educationSynchronizationOAuth1ConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="c1c02-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="c1c02-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1c02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1c02-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1c02-106">При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="c1c02-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="c1c02-107">На основе [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c1c02-107">Derived from [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1c02-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1c02-108">Properties</span></span>

<span data-ttu-id="c1c02-109">Дополнительные свойства, предоставляемые интерфейсом этого типа.</span><span class="sxs-lookup"><span data-stu-id="c1c02-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1c02-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1c02-110">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
