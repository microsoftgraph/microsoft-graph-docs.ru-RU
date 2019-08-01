---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b2aab468a6638b2e3bb525fd54c6554f5a5694a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032083"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="414d2-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="414d2-103">auditActor resource type</span></span>

> <span data-ttu-id="414d2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="414d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="414d2-105">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="414d2-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="414d2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="414d2-106">Properties</span></span>
|<span data-ttu-id="414d2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="414d2-107">Property</span></span>|<span data-ttu-id="414d2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="414d2-108">Type</span></span>|<span data-ttu-id="414d2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="414d2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="414d2-110">type</span><span class="sxs-lookup"><span data-stu-id="414d2-110">type</span></span>|<span data-ttu-id="414d2-111">String</span><span class="sxs-lookup"><span data-stu-id="414d2-111">String</span></span>|<span data-ttu-id="414d2-112">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="414d2-112">Actor Type.</span></span>|
|<span data-ttu-id="414d2-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="414d2-113">userPermissions</span></span>|<span data-ttu-id="414d2-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="414d2-114">String collection</span></span>|<span data-ttu-id="414d2-115">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="414d2-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="414d2-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="414d2-116">applicationId</span></span>|<span data-ttu-id="414d2-117">String</span><span class="sxs-lookup"><span data-stu-id="414d2-117">String</span></span>|<span data-ttu-id="414d2-118">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="414d2-118">AAD Application Id.</span></span>|
|<span data-ttu-id="414d2-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="414d2-119">applicationDisplayName</span></span>|<span data-ttu-id="414d2-120">String</span><span class="sxs-lookup"><span data-stu-id="414d2-120">String</span></span>|<span data-ttu-id="414d2-121">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="414d2-121">Name of the Application.</span></span>|
|<span data-ttu-id="414d2-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="414d2-122">userPrincipalName</span></span>|<span data-ttu-id="414d2-123">Строка</span><span class="sxs-lookup"><span data-stu-id="414d2-123">String</span></span>|<span data-ttu-id="414d2-124">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="414d2-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="414d2-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="414d2-125">servicePrincipalName</span></span>|<span data-ttu-id="414d2-126">String</span><span class="sxs-lookup"><span data-stu-id="414d2-126">String</span></span>|<span data-ttu-id="414d2-127">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="414d2-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="414d2-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="414d2-128">ipAddress</span></span>|<span data-ttu-id="414d2-129">String</span><span class="sxs-lookup"><span data-stu-id="414d2-129">String</span></span>|<span data-ttu-id="414d2-130">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="414d2-130">IPAddress.</span></span>|
|<span data-ttu-id="414d2-131">userId</span><span class="sxs-lookup"><span data-stu-id="414d2-131">userId</span></span>|<span data-ttu-id="414d2-132">String</span><span class="sxs-lookup"><span data-stu-id="414d2-132">String</span></span>|<span data-ttu-id="414d2-133">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="414d2-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="414d2-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="414d2-134">Relationships</span></span>
<span data-ttu-id="414d2-135">Нет</span><span class="sxs-lookup"><span data-stu-id="414d2-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="414d2-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="414d2-136">JSON Representation</span></span>
<span data-ttu-id="414d2-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="414d2-137">Here is a JSON representation of the resource.</span></span>
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



