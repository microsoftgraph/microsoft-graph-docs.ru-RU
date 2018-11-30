---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователей и групп сущностей при синхронизации каталогов в локальной для Azure Active Directory.
ms.openlocfilehash: 7d5b15d99559ddf5b7692b7eac9664de7ec50f1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028387"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="dcf40-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="dcf40-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="dcf40-104">Представляет ошибок синхронизации службы каталогов для [пользователей](user.md) и [групп](group.md) сущностей при синхронизации локальных каталогов в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dcf40-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="dcf40-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcf40-105">Properties</span></span>

| <span data-ttu-id="dcf40-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcf40-106">Property</span></span> | <span data-ttu-id="dcf40-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dcf40-107">Type</span></span> | <span data-ttu-id="dcf40-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf40-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dcf40-109">category</span><span class="sxs-lookup"><span data-stu-id="dcf40-109">category</span></span>|<span data-ttu-id="dcf40-110">String</span><span class="sxs-lookup"><span data-stu-id="dcf40-110">String</span></span>| <span data-ttu-id="dcf40-111">Категория Ошибка подготовки.</span><span class="sxs-lookup"><span data-stu-id="dcf40-111">Category of the provisioning error.</span></span> <span data-ttu-id="dcf40-112">Примечание: В настоящее время доступно только один значений.</span><span class="sxs-lookup"><span data-stu-id="dcf40-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="dcf40-113">Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="dcf40-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="dcf40-114">Такое же значение для свойства содержат другие объекты.</span><span class="sxs-lookup"><span data-stu-id="dcf40-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="dcf40-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="dcf40-115">occurredDateTime</span></span>|<span data-ttu-id="dcf40-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcf40-116">DateTimeOffset</span></span>| <span data-ttu-id="dcf40-117">Дата и время, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="dcf40-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="dcf40-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="dcf40-118">propertyCausingError</span></span>|<span data-ttu-id="dcf40-119">String</span><span class="sxs-lookup"><span data-stu-id="dcf40-119">String</span></span>| <span data-ttu-id="dcf40-120">Имя свойства каталогов, вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="dcf40-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="dcf40-121">Текущий возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="dcf40-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="dcf40-122">value</span><span class="sxs-lookup"><span data-stu-id="dcf40-122">value</span></span>|<span data-ttu-id="dcf40-123">String</span><span class="sxs-lookup"><span data-stu-id="dcf40-123">String</span></span>| <span data-ttu-id="dcf40-124">Значение свойства, вызывая ошибки.</span><span class="sxs-lookup"><span data-stu-id="dcf40-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dcf40-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcf40-125">JSON representation</span></span>
<span data-ttu-id="dcf40-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcf40-126">Here is a JSON representation of the resource.</span></span>

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