---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7d93f3a14f3f6fd1515de9232d26718b7ec0af6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971433"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="f7783-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="f7783-103">auditActor resource type</span></span>

> <span data-ttu-id="f7783-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7783-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7783-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7783-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7783-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7783-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7783-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="f7783-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="f7783-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7783-108">Properties</span></span>
|<span data-ttu-id="f7783-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7783-109">Property</span></span>|<span data-ttu-id="f7783-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f7783-110">Type</span></span>|<span data-ttu-id="f7783-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f7783-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7783-112">type</span><span class="sxs-lookup"><span data-stu-id="f7783-112">type</span></span>|<span data-ttu-id="f7783-113">String</span><span class="sxs-lookup"><span data-stu-id="f7783-113">String</span></span>|<span data-ttu-id="f7783-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="f7783-114">Actor Type.</span></span>|
|<span data-ttu-id="f7783-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f7783-115">userPermissions</span></span>|<span data-ttu-id="f7783-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f7783-116">String collection</span></span>|<span data-ttu-id="f7783-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="f7783-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="f7783-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="f7783-118">applicationId</span></span>|<span data-ttu-id="f7783-119">String</span><span class="sxs-lookup"><span data-stu-id="f7783-119">String</span></span>|<span data-ttu-id="f7783-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="f7783-120">AAD Application Id.</span></span>|
|<span data-ttu-id="f7783-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7783-121">applicationDisplayName</span></span>|<span data-ttu-id="f7783-122">String</span><span class="sxs-lookup"><span data-stu-id="f7783-122">String</span></span>|<span data-ttu-id="f7783-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f7783-123">Name of the Application.</span></span>|
|<span data-ttu-id="f7783-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7783-124">userPrincipalName</span></span>|<span data-ttu-id="f7783-125">String</span><span class="sxs-lookup"><span data-stu-id="f7783-125">String</span></span>|<span data-ttu-id="f7783-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="f7783-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f7783-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7783-127">servicePrincipalName</span></span>|<span data-ttu-id="f7783-128">String</span><span class="sxs-lookup"><span data-stu-id="f7783-128">String</span></span>|<span data-ttu-id="f7783-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="f7783-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f7783-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f7783-130">ipAddress</span></span>|<span data-ttu-id="f7783-131">String</span><span class="sxs-lookup"><span data-stu-id="f7783-131">String</span></span>|<span data-ttu-id="f7783-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="f7783-132">IPAddress.</span></span>|
|<span data-ttu-id="f7783-133">userId</span><span class="sxs-lookup"><span data-stu-id="f7783-133">userId</span></span>|<span data-ttu-id="f7783-134">String</span><span class="sxs-lookup"><span data-stu-id="f7783-134">String</span></span>|<span data-ttu-id="f7783-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7783-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7783-136">Связи</span><span class="sxs-lookup"><span data-stu-id="f7783-136">Relationships</span></span>
<span data-ttu-id="f7783-137">Нет</span><span class="sxs-lookup"><span data-stu-id="f7783-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7783-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7783-138">JSON Representation</span></span>
<span data-ttu-id="f7783-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7783-139">Here is a JSON representation of the resource.</span></span>
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





