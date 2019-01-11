---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c6dddd2863f881c026eb848c643bdc55cbbb372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873915"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="5fe94-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="5fe94-103">auditActor resource type</span></span>

> <span data-ttu-id="5fe94-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5fe94-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fe94-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fe94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fe94-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5fe94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fe94-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="5fe94-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="5fe94-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fe94-108">Properties</span></span>
|<span data-ttu-id="5fe94-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fe94-109">Property</span></span>|<span data-ttu-id="5fe94-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5fe94-110">Type</span></span>|<span data-ttu-id="5fe94-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5fe94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fe94-112">type</span><span class="sxs-lookup"><span data-stu-id="5fe94-112">type</span></span>|<span data-ttu-id="5fe94-113">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-113">String</span></span>|<span data-ttu-id="5fe94-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="5fe94-114">Actor Type.</span></span>|
|<span data-ttu-id="5fe94-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="5fe94-115">userPermissions</span></span>|<span data-ttu-id="5fe94-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5fe94-116">String collection</span></span>|<span data-ttu-id="5fe94-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="5fe94-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="5fe94-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="5fe94-118">applicationId</span></span>|<span data-ttu-id="5fe94-119">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-119">String</span></span>|<span data-ttu-id="5fe94-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="5fe94-120">AAD Application Id.</span></span>|
|<span data-ttu-id="5fe94-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="5fe94-121">applicationDisplayName</span></span>|<span data-ttu-id="5fe94-122">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-122">String</span></span>|<span data-ttu-id="5fe94-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="5fe94-123">Name of the Application.</span></span>|
|<span data-ttu-id="5fe94-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5fe94-124">userPrincipalName</span></span>|<span data-ttu-id="5fe94-125">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-125">String</span></span>|<span data-ttu-id="5fe94-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="5fe94-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="5fe94-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="5fe94-127">servicePrincipalName</span></span>|<span data-ttu-id="5fe94-128">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-128">String</span></span>|<span data-ttu-id="5fe94-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="5fe94-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="5fe94-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5fe94-130">ipAddress</span></span>|<span data-ttu-id="5fe94-131">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-131">String</span></span>|<span data-ttu-id="5fe94-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="5fe94-132">IPAddress.</span></span>|
|<span data-ttu-id="5fe94-133">userId</span><span class="sxs-lookup"><span data-stu-id="5fe94-133">userId</span></span>|<span data-ttu-id="5fe94-134">String</span><span class="sxs-lookup"><span data-stu-id="5fe94-134">String</span></span>|<span data-ttu-id="5fe94-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="5fe94-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fe94-136">Связи</span><span class="sxs-lookup"><span data-stu-id="5fe94-136">Relationships</span></span>
<span data-ttu-id="5fe94-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5fe94-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5fe94-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fe94-138">JSON Representation</span></span>
<span data-ttu-id="5fe94-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe94-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```





