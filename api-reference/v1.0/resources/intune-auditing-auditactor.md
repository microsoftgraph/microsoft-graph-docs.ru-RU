---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 632e3018f606b62171461b4b1235ccdafc6b1b5a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584707"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="51fb0-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="51fb0-103">auditActor resource type</span></span>

> <span data-ttu-id="51fb0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51fb0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51fb0-105">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="51fb0-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="51fb0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51fb0-106">Properties</span></span>
|<span data-ttu-id="51fb0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51fb0-107">Property</span></span>|<span data-ttu-id="51fb0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51fb0-108">Type</span></span>|<span data-ttu-id="51fb0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51fb0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51fb0-110">type</span><span class="sxs-lookup"><span data-stu-id="51fb0-110">type</span></span>|<span data-ttu-id="51fb0-111">Строка</span><span class="sxs-lookup"><span data-stu-id="51fb0-111">String</span></span>|<span data-ttu-id="51fb0-112">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="51fb0-112">Actor Type.</span></span>|
|<span data-ttu-id="51fb0-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="51fb0-113">userPermissions</span></span>|<span data-ttu-id="51fb0-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="51fb0-114">String collection</span></span>|<span data-ttu-id="51fb0-115">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="51fb0-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="51fb0-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="51fb0-116">applicationId</span></span>|<span data-ttu-id="51fb0-117">String</span><span class="sxs-lookup"><span data-stu-id="51fb0-117">String</span></span>|<span data-ttu-id="51fb0-118">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="51fb0-118">AAD Application Id.</span></span>|
|<span data-ttu-id="51fb0-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="51fb0-119">applicationDisplayName</span></span>|<span data-ttu-id="51fb0-120">String</span><span class="sxs-lookup"><span data-stu-id="51fb0-120">String</span></span>|<span data-ttu-id="51fb0-121">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="51fb0-121">Name of the Application.</span></span>|
|<span data-ttu-id="51fb0-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51fb0-122">userPrincipalName</span></span>|<span data-ttu-id="51fb0-123">String</span><span class="sxs-lookup"><span data-stu-id="51fb0-123">String</span></span>|<span data-ttu-id="51fb0-124">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="51fb0-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="51fb0-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="51fb0-125">servicePrincipalName</span></span>|<span data-ttu-id="51fb0-126">String</span><span class="sxs-lookup"><span data-stu-id="51fb0-126">String</span></span>|<span data-ttu-id="51fb0-127">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="51fb0-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="51fb0-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="51fb0-128">ipAddress</span></span>|<span data-ttu-id="51fb0-129">String</span><span class="sxs-lookup"><span data-stu-id="51fb0-129">String</span></span>|<span data-ttu-id="51fb0-130">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="51fb0-130">IPAddress.</span></span>|
|<span data-ttu-id="51fb0-131">userId</span><span class="sxs-lookup"><span data-stu-id="51fb0-131">userId</span></span>|<span data-ttu-id="51fb0-132">String</span><span class="sxs-lookup"><span data-stu-id="51fb0-132">String</span></span>|<span data-ttu-id="51fb0-133">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="51fb0-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51fb0-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="51fb0-134">Relationships</span></span>
<span data-ttu-id="51fb0-135">Нет</span><span class="sxs-lookup"><span data-stu-id="51fb0-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51fb0-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51fb0-136">JSON Representation</span></span>
<span data-ttu-id="51fb0-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51fb0-137">Here is a JSON representation of the resource.</span></span>
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



