---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77150c7a2b883acc6857cd0866459fb9423dfa6c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798749"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="b437e-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="b437e-103">auditActor resource type</span></span>

> <span data-ttu-id="b437e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b437e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b437e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b437e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b437e-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="b437e-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="b437e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b437e-107">Properties</span></span>
|<span data-ttu-id="b437e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b437e-108">Property</span></span>|<span data-ttu-id="b437e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b437e-109">Type</span></span>|<span data-ttu-id="b437e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b437e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b437e-111">type</span><span class="sxs-lookup"><span data-stu-id="b437e-111">type</span></span>|<span data-ttu-id="b437e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b437e-112">String</span></span>|<span data-ttu-id="b437e-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="b437e-113">Actor Type.</span></span>|
|<span data-ttu-id="b437e-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b437e-114">userPermissions</span></span>|<span data-ttu-id="b437e-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b437e-115">String collection</span></span>|<span data-ttu-id="b437e-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="b437e-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b437e-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="b437e-117">applicationId</span></span>|<span data-ttu-id="b437e-118">String</span><span class="sxs-lookup"><span data-stu-id="b437e-118">String</span></span>|<span data-ttu-id="b437e-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="b437e-119">AAD Application Id.</span></span>|
|<span data-ttu-id="b437e-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b437e-120">applicationDisplayName</span></span>|<span data-ttu-id="b437e-121">String</span><span class="sxs-lookup"><span data-stu-id="b437e-121">String</span></span>|<span data-ttu-id="b437e-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="b437e-122">Name of the Application.</span></span>|
|<span data-ttu-id="b437e-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b437e-123">userPrincipalName</span></span>|<span data-ttu-id="b437e-124">String</span><span class="sxs-lookup"><span data-stu-id="b437e-124">String</span></span>|<span data-ttu-id="b437e-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="b437e-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b437e-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b437e-126">servicePrincipalName</span></span>|<span data-ttu-id="b437e-127">String</span><span class="sxs-lookup"><span data-stu-id="b437e-127">String</span></span>|<span data-ttu-id="b437e-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="b437e-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b437e-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b437e-129">ipAddress</span></span>|<span data-ttu-id="b437e-130">String</span><span class="sxs-lookup"><span data-stu-id="b437e-130">String</span></span>|<span data-ttu-id="b437e-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="b437e-131">IPAddress.</span></span>|
|<span data-ttu-id="b437e-132">userId</span><span class="sxs-lookup"><span data-stu-id="b437e-132">userId</span></span>|<span data-ttu-id="b437e-133">String</span><span class="sxs-lookup"><span data-stu-id="b437e-133">String</span></span>|<span data-ttu-id="b437e-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="b437e-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b437e-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="b437e-135">Relationships</span></span>
<span data-ttu-id="b437e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="b437e-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b437e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b437e-137">JSON Representation</span></span>
<span data-ttu-id="b437e-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b437e-138">Here is a JSON representation of the resource.</span></span>
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





