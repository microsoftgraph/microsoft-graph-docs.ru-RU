---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c10ac0a18f5bfcf68be56edc402c83d9882a8ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532735"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="f4652-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="f4652-103">auditActor resource type</span></span>

<span data-ttu-id="f4652-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4652-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4652-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4652-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4652-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="f4652-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="f4652-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4652-107">Properties</span></span>
|<span data-ttu-id="f4652-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4652-108">Property</span></span>|<span data-ttu-id="f4652-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f4652-109">Type</span></span>|<span data-ttu-id="f4652-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4652-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4652-111">type</span><span class="sxs-lookup"><span data-stu-id="f4652-111">type</span></span>|<span data-ttu-id="f4652-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f4652-112">String</span></span>|<span data-ttu-id="f4652-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="f4652-113">Actor Type.</span></span>|
|<span data-ttu-id="f4652-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f4652-114">userPermissions</span></span>|<span data-ttu-id="f4652-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4652-115">String collection</span></span>|<span data-ttu-id="f4652-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="f4652-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="f4652-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="f4652-117">applicationId</span></span>|<span data-ttu-id="f4652-118">Строка</span><span class="sxs-lookup"><span data-stu-id="f4652-118">String</span></span>|<span data-ttu-id="f4652-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="f4652-119">AAD Application Id.</span></span>|
|<span data-ttu-id="f4652-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4652-120">applicationDisplayName</span></span>|<span data-ttu-id="f4652-121">Строка</span><span class="sxs-lookup"><span data-stu-id="f4652-121">String</span></span>|<span data-ttu-id="f4652-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f4652-122">Name of the Application.</span></span>|
|<span data-ttu-id="f4652-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4652-123">userPrincipalName</span></span>|<span data-ttu-id="f4652-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f4652-124">String</span></span>|<span data-ttu-id="f4652-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="f4652-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f4652-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4652-126">servicePrincipalName</span></span>|<span data-ttu-id="f4652-127">Строка</span><span class="sxs-lookup"><span data-stu-id="f4652-127">String</span></span>|<span data-ttu-id="f4652-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="f4652-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f4652-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f4652-129">ipAddress</span></span>|<span data-ttu-id="f4652-130">String</span><span class="sxs-lookup"><span data-stu-id="f4652-130">String</span></span>|<span data-ttu-id="f4652-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="f4652-131">IPAddress.</span></span>|
|<span data-ttu-id="f4652-132">userId</span><span class="sxs-lookup"><span data-stu-id="f4652-132">userId</span></span>|<span data-ttu-id="f4652-133">String</span><span class="sxs-lookup"><span data-stu-id="f4652-133">String</span></span>|<span data-ttu-id="f4652-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4652-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4652-135">Связи</span><span class="sxs-lookup"><span data-stu-id="f4652-135">Relationships</span></span>
<span data-ttu-id="f4652-136">Нет</span><span class="sxs-lookup"><span data-stu-id="f4652-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4652-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4652-137">JSON Representation</span></span>
<span data-ttu-id="f4652-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4652-138">Here is a JSON representation of the resource.</span></span>
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




