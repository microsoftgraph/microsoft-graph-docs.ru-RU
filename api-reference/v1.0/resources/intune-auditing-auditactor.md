---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c6a51d99d712305292e17d19487d829bd2e09af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439534"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="85500-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="85500-103">auditActor resource type</span></span>

<span data-ttu-id="85500-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85500-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85500-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85500-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="85500-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="85500-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="85500-107">Properties</span></span>
|<span data-ttu-id="85500-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="85500-108">Property</span></span>|<span data-ttu-id="85500-109">Тип</span><span class="sxs-lookup"><span data-stu-id="85500-109">Type</span></span>|<span data-ttu-id="85500-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85500-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85500-111">type</span><span class="sxs-lookup"><span data-stu-id="85500-111">type</span></span>|<span data-ttu-id="85500-112">String</span><span class="sxs-lookup"><span data-stu-id="85500-112">String</span></span>|<span data-ttu-id="85500-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="85500-113">Actor Type.</span></span>|
|<span data-ttu-id="85500-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="85500-114">userPermissions</span></span>|<span data-ttu-id="85500-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="85500-115">String collection</span></span>|<span data-ttu-id="85500-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="85500-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="85500-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="85500-117">applicationId</span></span>|<span data-ttu-id="85500-118">String</span><span class="sxs-lookup"><span data-stu-id="85500-118">String</span></span>|<span data-ttu-id="85500-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="85500-119">AAD Application Id.</span></span>|
|<span data-ttu-id="85500-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="85500-120">applicationDisplayName</span></span>|<span data-ttu-id="85500-121">String</span><span class="sxs-lookup"><span data-stu-id="85500-121">String</span></span>|<span data-ttu-id="85500-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="85500-122">Name of the Application.</span></span>|
|<span data-ttu-id="85500-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85500-123">userPrincipalName</span></span>|<span data-ttu-id="85500-124">Строка</span><span class="sxs-lookup"><span data-stu-id="85500-124">String</span></span>|<span data-ttu-id="85500-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="85500-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="85500-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="85500-126">servicePrincipalName</span></span>|<span data-ttu-id="85500-127">String</span><span class="sxs-lookup"><span data-stu-id="85500-127">String</span></span>|<span data-ttu-id="85500-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="85500-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="85500-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="85500-129">ipAddress</span></span>|<span data-ttu-id="85500-130">String</span><span class="sxs-lookup"><span data-stu-id="85500-130">String</span></span>|<span data-ttu-id="85500-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="85500-131">IPAddress.</span></span>|
|<span data-ttu-id="85500-132">userId</span><span class="sxs-lookup"><span data-stu-id="85500-132">userId</span></span>|<span data-ttu-id="85500-133">String</span><span class="sxs-lookup"><span data-stu-id="85500-133">String</span></span>|<span data-ttu-id="85500-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="85500-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85500-135">Связи</span><span class="sxs-lookup"><span data-stu-id="85500-135">Relationships</span></span>
<span data-ttu-id="85500-136">Нет</span><span class="sxs-lookup"><span data-stu-id="85500-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85500-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85500-137">JSON Representation</span></span>
<span data-ttu-id="85500-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85500-138">Here is a JSON representation of the resource.</span></span>
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







