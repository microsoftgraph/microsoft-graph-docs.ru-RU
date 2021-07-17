---
title: тип ресурса acl
description: Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 171b53adc815638546bbdf71411c58d293c05de4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467482"
---
# <a name="acl-resource-type"></a><span data-ttu-id="f1b4c-103">тип ресурса acl</span><span class="sxs-lookup"><span data-stu-id="f1b4c-103">acl resource type</span></span>

<span data-ttu-id="f1b4c-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="f1b4c-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="f1b4c-105">Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-105">An access control entry for an item indexed by a Microsoft Search externalConnection.</span></span>

## <a name="properties"></a><span data-ttu-id="f1b4c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1b4c-106">Properties</span></span>
|<span data-ttu-id="f1b4c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1b4c-107">Property</span></span>|<span data-ttu-id="f1b4c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f1b4c-108">Type</span></span>|<span data-ttu-id="f1b4c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f1b4c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1b4c-110">accessType</span><span class="sxs-lookup"><span data-stu-id="f1b4c-110">accessType</span></span>|<span data-ttu-id="f1b4c-111">microsoft.graph.externalConnectors.accessType</span><span class="sxs-lookup"><span data-stu-id="f1b4c-111">microsoft.graph.externalConnectors.accessType</span></span>|<span data-ttu-id="f1b4c-112">Доступ, предоставленный удостоверению.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-112">The access granted to the identity.</span></span> <span data-ttu-id="f1b4c-113">Возможные значения: `grant`, `deny`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-113">Possible values are: `grant`, `deny`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f1b4c-114">type</span><span class="sxs-lookup"><span data-stu-id="f1b4c-114">type</span></span>|<span data-ttu-id="f1b4c-115">microsoft.graph.externalConnectors.aclType</span><span class="sxs-lookup"><span data-stu-id="f1b4c-115">microsoft.graph.externalConnectors.aclType</span></span>|<span data-ttu-id="f1b4c-116">Тип удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-116">The type of identity.</span></span> <span data-ttu-id="f1b4c-117">Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-117">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f1b4c-118">value</span><span class="sxs-lookup"><span data-stu-id="f1b4c-118">value</span></span>|<span data-ttu-id="f1b4c-119">String</span><span class="sxs-lookup"><span data-stu-id="f1b4c-119">String</span></span>|<span data-ttu-id="f1b4c-120">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-120">The unique identifer of the identity.</span></span> <span data-ttu-id="f1b4c-121">В случае Azure Active Directory удостоверений устанавливается идентификатор объекта пользователя, группы или клиента для пользователей, групп и всех `value` (и всех пользователейExceptGuests) соответственно.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-121">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="f1b4c-122">Если внешние группы `value` задают ID externalGroup</span><span class="sxs-lookup"><span data-stu-id="f1b4c-122">In case of external groups `value` is set to the ID of the externalGroup</span></span> |

## <a name="relationships"></a><span data-ttu-id="f1b4c-123">Связи</span><span class="sxs-lookup"><span data-stu-id="f1b4c-123">Relationships</span></span>
<span data-ttu-id="f1b4c-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1b4c-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f1b4c-125">JSON representation</span></span>
<span data-ttu-id="f1b4c-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1b4c-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}
-->
``` json
{
  "type": "String",
  "value": "String",
  "accessType": "String"
}
```

