---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для сущностей контактов пользователя, группы или организации при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568852"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="1e823-103">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="1e823-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e823-104">Представляет ошибки синхронизации каталогов для сущностей контактов [пользователя](user.md), [группы](group.md)или [Организации](orgcontact.md) при синхронизации локальных каталогов с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e823-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="1e823-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e823-105">Properties</span></span>

| <span data-ttu-id="1e823-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e823-106">Property</span></span> | <span data-ttu-id="1e823-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1e823-107">Type</span></span> | <span data-ttu-id="1e823-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1e823-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1e823-109">category</span><span class="sxs-lookup"><span data-stu-id="1e823-109">category</span></span>|<span data-ttu-id="1e823-110">String</span><span class="sxs-lookup"><span data-stu-id="1e823-110">String</span></span>| <span data-ttu-id="1e823-111">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="1e823-111">Category of the provisioning error.</span></span> <span data-ttu-id="1e823-112">Примечание. в настоящее время существует только одно возможное значение.</span><span class="sxs-lookup"><span data-stu-id="1e823-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="1e823-113">Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="1e823-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="1e823-114">Другие объекты содержат одно и то же значение свойства.</span><span class="sxs-lookup"><span data-stu-id="1e823-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="1e823-115">Оккурреддатетиме</span><span class="sxs-lookup"><span data-stu-id="1e823-115">occurredDateTime</span></span>|<span data-ttu-id="1e823-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e823-116">DateTimeOffset</span></span>| <span data-ttu-id="1e823-117">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="1e823-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="1e823-118">Пропертикаусинжеррор</span><span class="sxs-lookup"><span data-stu-id="1e823-118">propertyCausingError</span></span>|<span data-ttu-id="1e823-119">String</span><span class="sxs-lookup"><span data-stu-id="1e823-119">String</span></span>| <span data-ttu-id="1e823-120">Имя свойства каталога, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="1e823-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="1e823-121">Текущие возможные значения: *userPrincipalName* или *proxyAddress*</span><span class="sxs-lookup"><span data-stu-id="1e823-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="1e823-122">value</span><span class="sxs-lookup"><span data-stu-id="1e823-122">value</span></span>|<span data-ttu-id="1e823-123">String</span><span class="sxs-lookup"><span data-stu-id="1e823-123">String</span></span>| <span data-ttu-id="1e823-124">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="1e823-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e823-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e823-125">JSON representation</span></span>
<span data-ttu-id="1e823-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e823-126">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
