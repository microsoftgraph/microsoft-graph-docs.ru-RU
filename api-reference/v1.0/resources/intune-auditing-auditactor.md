---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97707795907665ffe65cfee94a53b5d36238c297
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032476"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="4bc94-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="4bc94-103">auditActor resource type</span></span>

<span data-ttu-id="4bc94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bc94-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bc94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc94-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="4bc94-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="4bc94-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bc94-107">Properties</span></span>
|<span data-ttu-id="4bc94-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bc94-108">Property</span></span>|<span data-ttu-id="4bc94-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4bc94-109">Type</span></span>|<span data-ttu-id="4bc94-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4bc94-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc94-111">type</span><span class="sxs-lookup"><span data-stu-id="4bc94-111">type</span></span>|<span data-ttu-id="4bc94-112">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-112">String</span></span>|<span data-ttu-id="4bc94-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="4bc94-113">Actor Type.</span></span>|
|<span data-ttu-id="4bc94-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="4bc94-114">userPermissions</span></span>|<span data-ttu-id="4bc94-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4bc94-115">String collection</span></span>|<span data-ttu-id="4bc94-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="4bc94-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="4bc94-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="4bc94-117">applicationId</span></span>|<span data-ttu-id="4bc94-118">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-118">String</span></span>|<span data-ttu-id="4bc94-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="4bc94-119">AAD Application Id.</span></span>|
|<span data-ttu-id="4bc94-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="4bc94-120">applicationDisplayName</span></span>|<span data-ttu-id="4bc94-121">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-121">String</span></span>|<span data-ttu-id="4bc94-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="4bc94-122">Name of the Application.</span></span>|
|<span data-ttu-id="4bc94-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4bc94-123">userPrincipalName</span></span>|<span data-ttu-id="4bc94-124">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-124">String</span></span>|<span data-ttu-id="4bc94-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="4bc94-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="4bc94-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="4bc94-126">servicePrincipalName</span></span>|<span data-ttu-id="4bc94-127">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-127">String</span></span>|<span data-ttu-id="4bc94-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="4bc94-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="4bc94-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4bc94-129">ipAddress</span></span>|<span data-ttu-id="4bc94-130">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-130">String</span></span>|<span data-ttu-id="4bc94-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="4bc94-131">IPAddress.</span></span>|
|<span data-ttu-id="4bc94-132">userId</span><span class="sxs-lookup"><span data-stu-id="4bc94-132">userId</span></span>|<span data-ttu-id="4bc94-133">String</span><span class="sxs-lookup"><span data-stu-id="4bc94-133">String</span></span>|<span data-ttu-id="4bc94-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="4bc94-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bc94-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4bc94-135">Relationships</span></span>
<span data-ttu-id="4bc94-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4bc94-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bc94-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bc94-137">JSON Representation</span></span>
<span data-ttu-id="4bc94-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bc94-138">Here is a JSON representation of the resource.</span></span>
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









