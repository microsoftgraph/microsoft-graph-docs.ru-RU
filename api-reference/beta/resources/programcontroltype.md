---
title: Тип ресурса programControlType
description: 'В Azure AD access дается обзор компонента, тип элемента управления программы используется, когда для связывания элемента управления в программу, чтобы указать тип доступа проверки элемента управления.  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519705"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="f98bc-103">Тип ресурса programControlType</span><span class="sxs-lookup"><span data-stu-id="f98bc-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f98bc-104">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD тип элемента управления программы используется при связывания элемента управления в программу, чтобы указать тип проверки доступа, управления.</span><span class="sxs-lookup"><span data-stu-id="f98bc-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="f98bc-105">Объекты типа программа управления создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.</span><span class="sxs-lookup"><span data-stu-id="f98bc-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f98bc-106">Типы элементов управления не дополнительные программы могут быть созданы.</span><span class="sxs-lookup"><span data-stu-id="f98bc-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f98bc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f98bc-107">Methods</span></span>

| <span data-ttu-id="f98bc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f98bc-108">Method</span></span>           | <span data-ttu-id="f98bc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f98bc-109">Return Type</span></span>    |<span data-ttu-id="f98bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f98bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f98bc-111">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f98bc-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="f98bc-112">[programControlType](programcontroltype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f98bc-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="f98bc-113">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="f98bc-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="f98bc-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="f98bc-114">Properties</span></span>
| <span data-ttu-id="f98bc-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f98bc-115">Property</span></span>     | <span data-ttu-id="f98bc-116">Тип</span><span class="sxs-lookup"><span data-stu-id="f98bc-116">Type</span></span>   |<span data-ttu-id="f98bc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f98bc-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f98bc-118">Идентификатор компонента назначенные программы типа элемента управления</span><span class="sxs-lookup"><span data-stu-id="f98bc-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f98bc-119">Имя типа элемента управления программы</span><span class="sxs-lookup"><span data-stu-id="f98bc-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f98bc-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="f98bc-120">Relationships</span></span>

<span data-ttu-id="f98bc-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="f98bc-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="f98bc-122">См. также</span><span class="sxs-lookup"><span data-stu-id="f98bc-122">See also</span></span>

| <span data-ttu-id="f98bc-123">Метод</span><span class="sxs-lookup"><span data-stu-id="f98bc-123">Method</span></span>           | <span data-ttu-id="f98bc-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f98bc-124">Return Type</span></span>    |<span data-ttu-id="f98bc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f98bc-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f98bc-126">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="f98bc-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="f98bc-127">programControl</span><span class="sxs-lookup"><span data-stu-id="f98bc-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="f98bc-128">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="f98bc-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f98bc-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f98bc-129">JSON representation</span></span>

<span data-ttu-id="f98bc-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f98bc-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontroltype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
