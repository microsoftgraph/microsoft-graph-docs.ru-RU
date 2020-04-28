---
title: Тип ресурса Пассвордсинглесигнонкредентиалсет
description: Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9191362f0e6c98d57c609445fbe1caf3bdd775a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522006"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="8915b-103">Тип ресурса Пассвордсинглесигнонкредентиалсет</span><span class="sxs-lookup"><span data-stu-id="8915b-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="8915b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8915b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8915b-105">Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.</span><span class="sxs-lookup"><span data-stu-id="8915b-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="8915b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8915b-106">Properties</span></span>

| <span data-ttu-id="8915b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8915b-107">Property</span></span>     | <span data-ttu-id="8915b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8915b-108">Type</span></span>        | <span data-ttu-id="8915b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8915b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8915b-110">записей</span><span class="sxs-lookup"><span data-stu-id="8915b-110">credentials</span></span>|<span data-ttu-id="8915b-111">Коллекция [учетных данных](credential.md)</span><span class="sxs-lookup"><span data-stu-id="8915b-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="8915b-112">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="8915b-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="8915b-113">id</span><span class="sxs-lookup"><span data-stu-id="8915b-113">id</span></span>|<span data-ttu-id="8915b-114">String</span><span class="sxs-lookup"><span data-stu-id="8915b-114">String</span></span>|<span data-ttu-id="8915b-115">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="8915b-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8915b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8915b-116">JSON representation</span></span>

<span data-ttu-id="8915b-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8915b-117">The following is a JSON representation of the resource.</span></span>

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
