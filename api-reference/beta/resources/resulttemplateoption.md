---
title: тип ресурса resultTemplateOption
description: Предоставляет параметры макетов отображения поиска для результатов поиска соединители визуализации.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 404051f4eeee68ca3d5f5eb3ac6b84a23a331515
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211373"
---
# <a name="resulttemplateoption-resource-type"></a><span data-ttu-id="cee13-103">тип ресурса resultTemplateOption</span><span class="sxs-lookup"><span data-stu-id="cee13-103">resultTemplateOption resource type</span></span>

<span data-ttu-id="cee13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cee13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cee13-105">Предоставляет параметры шаблонов результатов поиска для результатов поиска соединители отрисовки.</span><span class="sxs-lookup"><span data-stu-id="cee13-105">Provides the search result templates options for render connectors search results.</span></span>

## <a name="properties"></a><span data-ttu-id="cee13-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cee13-106">Properties</span></span>

| <span data-ttu-id="cee13-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cee13-107">Property</span></span>     | <span data-ttu-id="cee13-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cee13-108">Type</span></span>        | <span data-ttu-id="cee13-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cee13-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cee13-110">enableResultTemplate</span><span class="sxs-lookup"><span data-stu-id="cee13-110">enableResultTemplate</span></span>|<span data-ttu-id="cee13-111">Логический</span><span class="sxs-lookup"><span data-stu-id="cee13-111">Boolean</span></span>|<span data-ttu-id="cee13-112">Указывает, включены ли макеты отображения поиска.</span><span class="sxs-lookup"><span data-stu-id="cee13-112">Indicates whether search display layouts are enabled.</span></span> <span data-ttu-id="cee13-113">Если включено, пользователь получит шаблон результатов для отображения контента результатов поиска в **свойстве resultTemplates** [ответа.](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="cee13-113">If enabled, the user will get the result template to render the search results content in the **resultTemplates** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="cee13-114">Шаблон результатов основан на [адаптивных картах.](https://adaptivecards.io/)</span><span class="sxs-lookup"><span data-stu-id="cee13-114">The result template is based on [Adaptive Cards](https://adaptivecards.io/).</span></span> <span data-ttu-id="cee13-115">Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="cee13-115">This property is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cee13-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cee13-116">JSON representation</span></span>

<span data-ttu-id="cee13-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cee13-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplateOption",
  "baseType": null
}-->

```json
 {
    "enableResultTemplate": true
 }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplateOption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
