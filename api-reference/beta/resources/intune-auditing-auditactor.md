---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425801"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="059b7-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="059b7-103">auditActor resource type</span></span>

> <span data-ttu-id="059b7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="059b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="059b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="059b7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="059b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="059b7-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="059b7-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="059b7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="059b7-108">Properties</span></span>
|<span data-ttu-id="059b7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="059b7-109">Property</span></span>|<span data-ttu-id="059b7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="059b7-110">Type</span></span>|<span data-ttu-id="059b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="059b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="059b7-112">type</span><span class="sxs-lookup"><span data-stu-id="059b7-112">type</span></span>|<span data-ttu-id="059b7-113">String</span><span class="sxs-lookup"><span data-stu-id="059b7-113">String</span></span>|<span data-ttu-id="059b7-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="059b7-114">Actor Type.</span></span>|
|<span data-ttu-id="059b7-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="059b7-115">userPermissions</span></span>|<span data-ttu-id="059b7-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="059b7-116">String collection</span></span>|<span data-ttu-id="059b7-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="059b7-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="059b7-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="059b7-118">applicationId</span></span>|<span data-ttu-id="059b7-119">String</span><span class="sxs-lookup"><span data-stu-id="059b7-119">String</span></span>|<span data-ttu-id="059b7-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="059b7-120">AAD Application Id.</span></span>|
|<span data-ttu-id="059b7-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="059b7-121">applicationDisplayName</span></span>|<span data-ttu-id="059b7-122">String</span><span class="sxs-lookup"><span data-stu-id="059b7-122">String</span></span>|<span data-ttu-id="059b7-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="059b7-123">Name of the Application.</span></span>|
|<span data-ttu-id="059b7-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="059b7-124">userPrincipalName</span></span>|<span data-ttu-id="059b7-125">String</span><span class="sxs-lookup"><span data-stu-id="059b7-125">String</span></span>|<span data-ttu-id="059b7-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="059b7-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="059b7-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="059b7-127">servicePrincipalName</span></span>|<span data-ttu-id="059b7-128">String</span><span class="sxs-lookup"><span data-stu-id="059b7-128">String</span></span>|<span data-ttu-id="059b7-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="059b7-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="059b7-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="059b7-130">ipAddress</span></span>|<span data-ttu-id="059b7-131">String</span><span class="sxs-lookup"><span data-stu-id="059b7-131">String</span></span>|<span data-ttu-id="059b7-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="059b7-132">IPAddress.</span></span>|
|<span data-ttu-id="059b7-133">userId</span><span class="sxs-lookup"><span data-stu-id="059b7-133">userId</span></span>|<span data-ttu-id="059b7-134">String</span><span class="sxs-lookup"><span data-stu-id="059b7-134">String</span></span>|<span data-ttu-id="059b7-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="059b7-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="059b7-136">Связи</span><span class="sxs-lookup"><span data-stu-id="059b7-136">Relationships</span></span>
<span data-ttu-id="059b7-137">Нет</span><span class="sxs-lookup"><span data-stu-id="059b7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="059b7-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="059b7-138">JSON Representation</span></span>
<span data-ttu-id="059b7-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="059b7-139">Here is a JSON representation of the resource.</span></span>
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




