---
title: Тип ресурса Оненотеидентитисет
description: '**Поддержка скоро**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: c0d2f0b4ed65ac83a59036c362136b7af772d21c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290583"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="41528-103">Тип ресурса Оненотеидентитисет</span><span class="sxs-lookup"><span data-stu-id="41528-103">oneNoteIdentitySet resource type</span></span>

<span data-ttu-id="41528-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41528-105">**Поддержка скоро**</span><span class="sxs-lookup"><span data-stu-id="41528-105">**Support coming soon**</span></span>

<span data-ttu-id="41528-106">Тип Оненотеидентитисет является коллекцией с ключами объектов [оненотеидентити](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="41528-106">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="41528-107">Он используется для представления набора удостоверений, связанных с различными событиями для _записной книжки_, _раздела_ или _страницы_, например _созданных автором_ или _автором последнего изменения_.</span><span class="sxs-lookup"><span data-stu-id="41528-107">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="41528-108">В настоящее время он содержит один ключ, _**User**_.</span><span class="sxs-lookup"><span data-stu-id="41528-108">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="41528-109">В дальнейшем можно добавить такие ключи, как устройство или приложение для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="41528-109">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="41528-110">В дальнейшем этот тип будет объединен с [Identity](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="41528-110">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="41528-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41528-111">JSON representation</span></span>

<span data-ttu-id="41528-112">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41528-112">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="41528-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="41528-113">Properties</span></span>
| <span data-ttu-id="41528-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="41528-114">Property</span></span>     | <span data-ttu-id="41528-115">Тип</span><span class="sxs-lookup"><span data-stu-id="41528-115">Type</span></span>   |<span data-ttu-id="41528-116">Описание</span><span class="sxs-lookup"><span data-stu-id="41528-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41528-117">user</span><span class="sxs-lookup"><span data-stu-id="41528-117">user</span></span>|[<span data-ttu-id="41528-118">оненотеидентити</span><span class="sxs-lookup"><span data-stu-id="41528-118">onenoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="41528-119">Ресурс Оненотеидентити, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="41528-119">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
