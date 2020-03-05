---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40aa3d256da1d7a1c50fc898c6755a82185897ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489491"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="0cdcb-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="0cdcb-103">auditActor resource type</span></span>

<span data-ttu-id="0cdcb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0cdcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cdcb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cdcb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cdcb-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="0cdcb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cdcb-108">Properties</span></span>
|<span data-ttu-id="0cdcb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cdcb-109">Property</span></span>|<span data-ttu-id="0cdcb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0cdcb-110">Type</span></span>|<span data-ttu-id="0cdcb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0cdcb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cdcb-112">type</span><span class="sxs-lookup"><span data-stu-id="0cdcb-112">type</span></span>|<span data-ttu-id="0cdcb-113">String</span><span class="sxs-lookup"><span data-stu-id="0cdcb-113">String</span></span>|<span data-ttu-id="0cdcb-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-114">Actor Type.</span></span>|
|<span data-ttu-id="0cdcb-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="0cdcb-115">userPermissions</span></span>|<span data-ttu-id="0cdcb-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0cdcb-116">String collection</span></span>|<span data-ttu-id="0cdcb-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="0cdcb-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="0cdcb-118">applicationId</span></span>|<span data-ttu-id="0cdcb-119">String</span><span class="sxs-lookup"><span data-stu-id="0cdcb-119">String</span></span>|<span data-ttu-id="0cdcb-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-120">AAD Application Id.</span></span>|
|<span data-ttu-id="0cdcb-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="0cdcb-121">applicationDisplayName</span></span>|<span data-ttu-id="0cdcb-122">String</span><span class="sxs-lookup"><span data-stu-id="0cdcb-122">String</span></span>|<span data-ttu-id="0cdcb-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-123">Name of the Application.</span></span>|
|<span data-ttu-id="0cdcb-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0cdcb-124">userPrincipalName</span></span>|<span data-ttu-id="0cdcb-125">Строка</span><span class="sxs-lookup"><span data-stu-id="0cdcb-125">String</span></span>|<span data-ttu-id="0cdcb-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="0cdcb-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="0cdcb-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="0cdcb-127">servicePrincipalName</span></span>|<span data-ttu-id="0cdcb-128">String</span><span class="sxs-lookup"><span data-stu-id="0cdcb-128">String</span></span>|<span data-ttu-id="0cdcb-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="0cdcb-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="0cdcb-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0cdcb-130">ipAddress</span></span>|<span data-ttu-id="0cdcb-131">String</span><span class="sxs-lookup"><span data-stu-id="0cdcb-131">String</span></span>|<span data-ttu-id="0cdcb-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-132">IPAddress.</span></span>|
|<span data-ttu-id="0cdcb-133">userId</span><span class="sxs-lookup"><span data-stu-id="0cdcb-133">userId</span></span>|<span data-ttu-id="0cdcb-134">String</span><span class="sxs-lookup"><span data-stu-id="0cdcb-134">String</span></span>|<span data-ttu-id="0cdcb-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-135">User Id.</span></span>|
|<span data-ttu-id="0cdcb-136">усерролескопетагс</span><span class="sxs-lookup"><span data-stu-id="0cdcb-136">userRoleScopeTags</span></span>|<span data-ttu-id="0cdcb-137">Коллекция [ролескопетагинфо](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="0cdcb-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="0cdcb-138">Список тегов области пользователя при выполнении аудита.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-138">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cdcb-139">Связи</span><span class="sxs-lookup"><span data-stu-id="0cdcb-139">Relationships</span></span>
<span data-ttu-id="0cdcb-140">Нет</span><span class="sxs-lookup"><span data-stu-id="0cdcb-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cdcb-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cdcb-141">JSON Representation</span></span>
<span data-ttu-id="0cdcb-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cdcb-142">Here is a JSON representation of the resource.</span></span>
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
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ]
}
```



