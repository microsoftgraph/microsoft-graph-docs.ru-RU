---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации службы каталогов для группы пользователей и контактных ресурсов при синхронизации локального каталога с Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2647e32653d26793b4f875bb47ce43e83a294c4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133332"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="21d38-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="21d38-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="21d38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21d38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21d38-105">Представляет ошибки синхронизации службы каталогов для ресурсов [user,](user.md) [group](group.md) и [orgContact](orgcontact.md) при синхронизации локального каталога с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="21d38-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="21d38-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="21d38-106">Properties</span></span>

| <span data-ttu-id="21d38-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="21d38-107">Property</span></span> | <span data-ttu-id="21d38-108">Тип</span><span class="sxs-lookup"><span data-stu-id="21d38-108">Type</span></span> | <span data-ttu-id="21d38-109">Описание</span><span class="sxs-lookup"><span data-stu-id="21d38-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="21d38-110">category</span><span class="sxs-lookup"><span data-stu-id="21d38-110">category</span></span>|<span data-ttu-id="21d38-111">String</span><span class="sxs-lookup"><span data-stu-id="21d38-111">String</span></span>| <span data-ttu-id="21d38-112">Категория ошибки при предоставлении.</span><span class="sxs-lookup"><span data-stu-id="21d38-112">Category of the provisioning error.</span></span> <span data-ttu-id="21d38-113">Примечание. В настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="21d38-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="21d38-114">Возможное значение: *PropertyConflict* — указывает, что значение свойства не уникально.</span><span class="sxs-lookup"><span data-stu-id="21d38-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="21d38-115">Другие объекты содержат такое же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="21d38-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="21d38-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="21d38-116">occurredDateTime</span></span>|<span data-ttu-id="21d38-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21d38-117">DateTimeOffset</span></span>| <span data-ttu-id="21d38-118">Дата и время, когда произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="21d38-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="21d38-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="21d38-119">propertyCausingError</span></span>|<span data-ttu-id="21d38-120">String</span><span class="sxs-lookup"><span data-stu-id="21d38-120">String</span></span>| <span data-ttu-id="21d38-121">Имя свойства каталога, вызываемого ошибкой.</span><span class="sxs-lookup"><span data-stu-id="21d38-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="21d38-122">Текущие возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="21d38-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="21d38-123">value</span><span class="sxs-lookup"><span data-stu-id="21d38-123">value</span></span>|<span data-ttu-id="21d38-124">String</span><span class="sxs-lookup"><span data-stu-id="21d38-124">String</span></span>| <span data-ttu-id="21d38-125">Значение свойства, вызываемого ошибкой.</span><span class="sxs-lookup"><span data-stu-id="21d38-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="21d38-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21d38-126">JSON representation</span></span>
<span data-ttu-id="21d38-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21d38-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

