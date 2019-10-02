---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4365daebf50de210482132354c14199c850e384a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355997"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="d8031-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="d8031-103">auditActor resource type</span></span>

> <span data-ttu-id="d8031-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8031-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8031-105">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="d8031-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="d8031-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8031-106">Properties</span></span>
|<span data-ttu-id="d8031-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8031-107">Property</span></span>|<span data-ttu-id="d8031-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d8031-108">Type</span></span>|<span data-ttu-id="d8031-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d8031-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8031-110">type</span><span class="sxs-lookup"><span data-stu-id="d8031-110">type</span></span>|<span data-ttu-id="d8031-111">String</span><span class="sxs-lookup"><span data-stu-id="d8031-111">String</span></span>|<span data-ttu-id="d8031-112">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="d8031-112">Actor Type.</span></span>|
|<span data-ttu-id="d8031-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="d8031-113">userPermissions</span></span>|<span data-ttu-id="d8031-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d8031-114">String collection</span></span>|<span data-ttu-id="d8031-115">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="d8031-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="d8031-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="d8031-116">applicationId</span></span>|<span data-ttu-id="d8031-117">String</span><span class="sxs-lookup"><span data-stu-id="d8031-117">String</span></span>|<span data-ttu-id="d8031-118">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="d8031-118">AAD Application Id.</span></span>|
|<span data-ttu-id="d8031-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8031-119">applicationDisplayName</span></span>|<span data-ttu-id="d8031-120">String</span><span class="sxs-lookup"><span data-stu-id="d8031-120">String</span></span>|<span data-ttu-id="d8031-121">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d8031-121">Name of the Application.</span></span>|
|<span data-ttu-id="d8031-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8031-122">userPrincipalName</span></span>|<span data-ttu-id="d8031-123">Строка</span><span class="sxs-lookup"><span data-stu-id="d8031-123">String</span></span>|<span data-ttu-id="d8031-124">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="d8031-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="d8031-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8031-125">servicePrincipalName</span></span>|<span data-ttu-id="d8031-126">String</span><span class="sxs-lookup"><span data-stu-id="d8031-126">String</span></span>|<span data-ttu-id="d8031-127">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="d8031-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="d8031-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d8031-128">ipAddress</span></span>|<span data-ttu-id="d8031-129">String</span><span class="sxs-lookup"><span data-stu-id="d8031-129">String</span></span>|<span data-ttu-id="d8031-130">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="d8031-130">IPAddress.</span></span>|
|<span data-ttu-id="d8031-131">userId</span><span class="sxs-lookup"><span data-stu-id="d8031-131">userId</span></span>|<span data-ttu-id="d8031-132">String</span><span class="sxs-lookup"><span data-stu-id="d8031-132">String</span></span>|<span data-ttu-id="d8031-133">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="d8031-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8031-134">Связи</span><span class="sxs-lookup"><span data-stu-id="d8031-134">Relationships</span></span>
<span data-ttu-id="d8031-135">Нет</span><span class="sxs-lookup"><span data-stu-id="d8031-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8031-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8031-136">JSON Representation</span></span>
<span data-ttu-id="d8031-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8031-137">Here is a JSON representation of the resource.</span></span>
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




