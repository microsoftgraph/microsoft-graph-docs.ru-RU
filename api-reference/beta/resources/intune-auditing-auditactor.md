---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 633f5f4c513d6f770df643c26934b994a134e450
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985621"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="02a21-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="02a21-103">auditActor resource type</span></span>

> <span data-ttu-id="02a21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02a21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02a21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02a21-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="02a21-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="02a21-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="02a21-107">Properties</span></span>
|<span data-ttu-id="02a21-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="02a21-108">Property</span></span>|<span data-ttu-id="02a21-109">Тип</span><span class="sxs-lookup"><span data-stu-id="02a21-109">Type</span></span>|<span data-ttu-id="02a21-110">Описание</span><span class="sxs-lookup"><span data-stu-id="02a21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a21-111">type</span><span class="sxs-lookup"><span data-stu-id="02a21-111">type</span></span>|<span data-ttu-id="02a21-112">String</span><span class="sxs-lookup"><span data-stu-id="02a21-112">String</span></span>|<span data-ttu-id="02a21-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="02a21-113">Actor Type.</span></span>|
|<span data-ttu-id="02a21-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="02a21-114">userPermissions</span></span>|<span data-ttu-id="02a21-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02a21-115">String collection</span></span>|<span data-ttu-id="02a21-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="02a21-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="02a21-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="02a21-117">applicationId</span></span>|<span data-ttu-id="02a21-118">String</span><span class="sxs-lookup"><span data-stu-id="02a21-118">String</span></span>|<span data-ttu-id="02a21-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="02a21-119">AAD Application Id.</span></span>|
|<span data-ttu-id="02a21-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="02a21-120">applicationDisplayName</span></span>|<span data-ttu-id="02a21-121">String</span><span class="sxs-lookup"><span data-stu-id="02a21-121">String</span></span>|<span data-ttu-id="02a21-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="02a21-122">Name of the Application.</span></span>|
|<span data-ttu-id="02a21-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02a21-123">userPrincipalName</span></span>|<span data-ttu-id="02a21-124">Строка</span><span class="sxs-lookup"><span data-stu-id="02a21-124">String</span></span>|<span data-ttu-id="02a21-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="02a21-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="02a21-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="02a21-126">servicePrincipalName</span></span>|<span data-ttu-id="02a21-127">String</span><span class="sxs-lookup"><span data-stu-id="02a21-127">String</span></span>|<span data-ttu-id="02a21-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="02a21-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="02a21-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="02a21-129">ipAddress</span></span>|<span data-ttu-id="02a21-130">String</span><span class="sxs-lookup"><span data-stu-id="02a21-130">String</span></span>|<span data-ttu-id="02a21-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="02a21-131">IPAddress.</span></span>|
|<span data-ttu-id="02a21-132">userId</span><span class="sxs-lookup"><span data-stu-id="02a21-132">userId</span></span>|<span data-ttu-id="02a21-133">String</span><span class="sxs-lookup"><span data-stu-id="02a21-133">String</span></span>|<span data-ttu-id="02a21-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="02a21-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02a21-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="02a21-135">Relationships</span></span>
<span data-ttu-id="02a21-136">Нет</span><span class="sxs-lookup"><span data-stu-id="02a21-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02a21-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02a21-137">JSON Representation</span></span>
<span data-ttu-id="02a21-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02a21-138">Here is a JSON representation of the resource.</span></span>
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





