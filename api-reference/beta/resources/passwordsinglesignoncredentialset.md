---
title: Тип ресурса Пассвордсинглесигнонкредентиалсет
description: Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6293c6a2fbdffd124a8e011bd00a22c30efa77e5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658795"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="4dc0f-103">Тип ресурса Пассвордсинглесигнонкредентиалсет</span><span class="sxs-lookup"><span data-stu-id="4dc0f-103">passwordSingleSignOnCredentialSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc0f-104">Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.</span><span class="sxs-lookup"><span data-stu-id="4dc0f-104">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="4dc0f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dc0f-105">Properties</span></span>

| <span data-ttu-id="4dc0f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dc0f-106">Property</span></span>     | <span data-ttu-id="4dc0f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4dc0f-107">Type</span></span>        | <span data-ttu-id="4dc0f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc0f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4dc0f-109">записей</span><span class="sxs-lookup"><span data-stu-id="4dc0f-109">credentials</span></span>|<span data-ttu-id="4dc0f-110">Коллекция [учетных данных](credential.md)</span><span class="sxs-lookup"><span data-stu-id="4dc0f-110">[credential](credential.md) collection</span></span>|<span data-ttu-id="4dc0f-111">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="4dc0f-111">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="4dc0f-112">id</span><span class="sxs-lookup"><span data-stu-id="4dc0f-112">id</span></span>|<span data-ttu-id="4dc0f-113">String</span><span class="sxs-lookup"><span data-stu-id="4dc0f-113">String</span></span>|<span data-ttu-id="4dc0f-114">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4dc0f-114">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4dc0f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dc0f-115">JSON representation</span></span>

<span data-ttu-id="4dc0f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dc0f-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet",
  "baseType": null
}-->

```json
{
  "credentials": [{"@odata.type": "microsoft.graph.credential"}],
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnCredentialSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
