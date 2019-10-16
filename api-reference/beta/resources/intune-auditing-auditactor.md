---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fdb804dc293214fbcd7d937adb9ebdf959ea5fa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538520"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="20d40-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="20d40-103">auditActor resource type</span></span>

> <span data-ttu-id="20d40-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20d40-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20d40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20d40-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="20d40-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="20d40-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="20d40-107">Properties</span></span>
|<span data-ttu-id="20d40-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="20d40-108">Property</span></span>|<span data-ttu-id="20d40-109">Тип</span><span class="sxs-lookup"><span data-stu-id="20d40-109">Type</span></span>|<span data-ttu-id="20d40-110">Описание</span><span class="sxs-lookup"><span data-stu-id="20d40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20d40-111">type</span><span class="sxs-lookup"><span data-stu-id="20d40-111">type</span></span>|<span data-ttu-id="20d40-112">String</span><span class="sxs-lookup"><span data-stu-id="20d40-112">String</span></span>|<span data-ttu-id="20d40-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="20d40-113">Actor Type.</span></span>|
|<span data-ttu-id="20d40-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="20d40-114">userPermissions</span></span>|<span data-ttu-id="20d40-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20d40-115">String collection</span></span>|<span data-ttu-id="20d40-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="20d40-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="20d40-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="20d40-117">applicationId</span></span>|<span data-ttu-id="20d40-118">String</span><span class="sxs-lookup"><span data-stu-id="20d40-118">String</span></span>|<span data-ttu-id="20d40-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="20d40-119">AAD Application Id.</span></span>|
|<span data-ttu-id="20d40-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="20d40-120">applicationDisplayName</span></span>|<span data-ttu-id="20d40-121">String</span><span class="sxs-lookup"><span data-stu-id="20d40-121">String</span></span>|<span data-ttu-id="20d40-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="20d40-122">Name of the Application.</span></span>|
|<span data-ttu-id="20d40-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="20d40-123">userPrincipalName</span></span>|<span data-ttu-id="20d40-124">Строка</span><span class="sxs-lookup"><span data-stu-id="20d40-124">String</span></span>|<span data-ttu-id="20d40-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="20d40-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="20d40-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="20d40-126">servicePrincipalName</span></span>|<span data-ttu-id="20d40-127">String</span><span class="sxs-lookup"><span data-stu-id="20d40-127">String</span></span>|<span data-ttu-id="20d40-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="20d40-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="20d40-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="20d40-129">ipAddress</span></span>|<span data-ttu-id="20d40-130">String</span><span class="sxs-lookup"><span data-stu-id="20d40-130">String</span></span>|<span data-ttu-id="20d40-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="20d40-131">IPAddress.</span></span>|
|<span data-ttu-id="20d40-132">userId</span><span class="sxs-lookup"><span data-stu-id="20d40-132">userId</span></span>|<span data-ttu-id="20d40-133">String</span><span class="sxs-lookup"><span data-stu-id="20d40-133">String</span></span>|<span data-ttu-id="20d40-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="20d40-134">User Id.</span></span>|
|<span data-ttu-id="20d40-135">скопетагс</span><span class="sxs-lookup"><span data-stu-id="20d40-135">scopeTags</span></span>|<span data-ttu-id="20d40-136">Коллекция [скопетагинфо](../resources/intune-auditing-scopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="20d40-136">[scopeTagInfo](../resources/intune-auditing-scopetaginfo.md) collection</span></span>|<span data-ttu-id="20d40-137">Список тегов области пользователя при выполнении аудита.</span><span class="sxs-lookup"><span data-stu-id="20d40-137">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20d40-138">Связи</span><span class="sxs-lookup"><span data-stu-id="20d40-138">Relationships</span></span>
<span data-ttu-id="20d40-139">Нет</span><span class="sxs-lookup"><span data-stu-id="20d40-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20d40-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20d40-140">JSON Representation</span></span>
<span data-ttu-id="20d40-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20d40-141">Here is a JSON representation of the resource.</span></span>
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
  "scopeTags": [
    {
      "@odata.type": "microsoft.graph.scopeTagInfo",
      "scopeTagName": "String",
      "scopeTagId": "String"
    }
  ]
}
```



