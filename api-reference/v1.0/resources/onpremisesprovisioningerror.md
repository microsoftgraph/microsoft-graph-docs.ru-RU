---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователей и групп сущностей при синхронизации каталогов в локальной для Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830669"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="6da77-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="6da77-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="6da77-104">Представляет ошибок синхронизации службы каталогов для [пользователей](user.md) и [групп](group.md) сущностей при синхронизации локальных каталогов в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6da77-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="6da77-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6da77-105">Properties</span></span>

| <span data-ttu-id="6da77-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6da77-106">Property</span></span> | <span data-ttu-id="6da77-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6da77-107">Type</span></span> | <span data-ttu-id="6da77-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6da77-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6da77-109">category</span><span class="sxs-lookup"><span data-stu-id="6da77-109">category</span></span>|<span data-ttu-id="6da77-110">String</span><span class="sxs-lookup"><span data-stu-id="6da77-110">String</span></span>| <span data-ttu-id="6da77-111">Категория Ошибка подготовки.</span><span class="sxs-lookup"><span data-stu-id="6da77-111">Category of the provisioning error.</span></span> <span data-ttu-id="6da77-112">Примечание: В настоящее время доступно только один значений.</span><span class="sxs-lookup"><span data-stu-id="6da77-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="6da77-113">Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="6da77-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="6da77-114">Такое же значение для свойства содержат другие объекты.</span><span class="sxs-lookup"><span data-stu-id="6da77-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="6da77-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="6da77-115">occurredDateTime</span></span>|<span data-ttu-id="6da77-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da77-116">DateTimeOffset</span></span>| <span data-ttu-id="6da77-117">Дата и время, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="6da77-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="6da77-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="6da77-118">propertyCausingError</span></span>|<span data-ttu-id="6da77-119">Строка</span><span class="sxs-lookup"><span data-stu-id="6da77-119">String</span></span>| <span data-ttu-id="6da77-120">Имя свойства каталогов, вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="6da77-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="6da77-121">Текущий возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="6da77-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="6da77-122">value</span><span class="sxs-lookup"><span data-stu-id="6da77-122">value</span></span>|<span data-ttu-id="6da77-123">Строка</span><span class="sxs-lookup"><span data-stu-id="6da77-123">String</span></span>| <span data-ttu-id="6da77-124">Значение свойства, вызывая ошибки.</span><span class="sxs-lookup"><span data-stu-id="6da77-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6da77-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6da77-125">JSON representation</span></span>
<span data-ttu-id="6da77-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da77-126">Here is a JSON representation of the resource.</span></span>

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
