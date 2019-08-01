---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для сущностей пользователей и групп при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3fd16b43d35cb12e7b9c7f82dc59f940994bc1b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035750"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="4d3d6-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="4d3d6-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="4d3d6-104">Представляет ошибки синхронизации каталогов для сущностей [пользователей](user.md) и [групп](group.md) при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="4d3d6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d3d6-105">Properties</span></span>

| <span data-ttu-id="4d3d6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d3d6-106">Property</span></span> | <span data-ttu-id="4d3d6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4d3d6-107">Type</span></span> | <span data-ttu-id="4d3d6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4d3d6-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4d3d6-109">category</span><span class="sxs-lookup"><span data-stu-id="4d3d6-109">category</span></span>|<span data-ttu-id="4d3d6-110">String</span><span class="sxs-lookup"><span data-stu-id="4d3d6-110">String</span></span>| <span data-ttu-id="4d3d6-111">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-111">Category of the provisioning error.</span></span> <span data-ttu-id="4d3d6-112">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="4d3d6-113">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="4d3d6-114">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="4d3d6-115">Оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="4d3d6-115">occurredDateTime</span></span>|<span data-ttu-id="4d3d6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d3d6-116">DateTimeOffset</span></span>| <span data-ttu-id="4d3d6-117">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="4d3d6-118">Пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="4d3d6-118">propertyCausingError</span></span>|<span data-ttu-id="4d3d6-119">String</span><span class="sxs-lookup"><span data-stu-id="4d3d6-119">String</span></span>| <span data-ttu-id="4d3d6-120">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="4d3d6-121">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="4d3d6-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="4d3d6-122">value</span><span class="sxs-lookup"><span data-stu-id="4d3d6-122">value</span></span>|<span data-ttu-id="4d3d6-123">String</span><span class="sxs-lookup"><span data-stu-id="4d3d6-123">String</span></span>| <span data-ttu-id="4d3d6-124">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d3d6-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d3d6-125">JSON representation</span></span>
<span data-ttu-id="4d3d6-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d3d6-126">Here is a JSON representation of the resource.</span></span>

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
