---
title: educationSynchronizationOAuth1ConnectionSettings ресурсов
description: При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
ms.openlocfilehash: 17bfbed14bf22d8b30d82766985d64595204d05b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080523"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="3a291-103">educationSynchronizationOAuth1ConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="3a291-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="3a291-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a291-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a291-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a291-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a291-106">При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="3a291-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="3a291-107">На основе [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3a291-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3a291-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a291-108">Properties</span></span>

<span data-ttu-id="3a291-109">Дополнительные свойства, предоставляемые интерфейсом этого типа.</span><span class="sxs-lookup"><span data-stu-id="3a291-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a291-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a291-110">JSON representation</span></span>
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
