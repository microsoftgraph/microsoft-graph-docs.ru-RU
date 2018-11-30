---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
ms.openlocfilehash: f8a2858854a8efb07cd710c5bccb718dd504a81e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074569"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="d6f15-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="d6f15-103">auditActor resource type</span></span>

> <span data-ttu-id="d6f15-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6f15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6f15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6f15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6f15-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6f15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6f15-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="d6f15-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="d6f15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6f15-108">Properties</span></span>
|<span data-ttu-id="d6f15-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6f15-109">Property</span></span>|<span data-ttu-id="d6f15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d6f15-110">Type</span></span>|<span data-ttu-id="d6f15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6f15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6f15-112">type</span><span class="sxs-lookup"><span data-stu-id="d6f15-112">type</span></span>|<span data-ttu-id="d6f15-113">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-113">String</span></span>|<span data-ttu-id="d6f15-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="d6f15-114">Actor Type.</span></span>|
|<span data-ttu-id="d6f15-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="d6f15-115">userPermissions</span></span>|<span data-ttu-id="d6f15-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6f15-116">String collection</span></span>|<span data-ttu-id="d6f15-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="d6f15-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="d6f15-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="d6f15-118">applicationId</span></span>|<span data-ttu-id="d6f15-119">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-119">String</span></span>|<span data-ttu-id="d6f15-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="d6f15-120">AAD Application Id.</span></span>|
|<span data-ttu-id="d6f15-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6f15-121">applicationDisplayName</span></span>|<span data-ttu-id="d6f15-122">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-122">String</span></span>|<span data-ttu-id="d6f15-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d6f15-123">Name of the Application.</span></span>|
|<span data-ttu-id="d6f15-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6f15-124">userPrincipalName</span></span>|<span data-ttu-id="d6f15-125">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-125">String</span></span>|<span data-ttu-id="d6f15-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="d6f15-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="d6f15-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6f15-127">servicePrincipalName</span></span>|<span data-ttu-id="d6f15-128">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-128">String</span></span>|<span data-ttu-id="d6f15-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="d6f15-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="d6f15-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d6f15-130">ipAddress</span></span>|<span data-ttu-id="d6f15-131">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-131">String</span></span>|<span data-ttu-id="d6f15-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="d6f15-132">IPAddress.</span></span>|
|<span data-ttu-id="d6f15-133">userId</span><span class="sxs-lookup"><span data-stu-id="d6f15-133">userId</span></span>|<span data-ttu-id="d6f15-134">String</span><span class="sxs-lookup"><span data-stu-id="d6f15-134">String</span></span>|<span data-ttu-id="d6f15-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6f15-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6f15-136">Связи</span><span class="sxs-lookup"><span data-stu-id="d6f15-136">Relationships</span></span>
<span data-ttu-id="d6f15-137">Нет</span><span class="sxs-lookup"><span data-stu-id="d6f15-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6f15-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6f15-138">JSON Representation</span></span>
<span data-ttu-id="d6f15-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6f15-139">Here is a JSON representation of the resource.</span></span>
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





