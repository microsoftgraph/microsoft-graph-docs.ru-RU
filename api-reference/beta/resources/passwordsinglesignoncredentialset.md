---
title: Тип ресурса Пассвордсинглесигнонкредентиалсет
description: Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87aafa6e21171088f9b4b5eac318f6c9551e18ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998203"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="7a885-103">Тип ресурса Пассвордсинглесигнонкредентиалсет</span><span class="sxs-lookup"><span data-stu-id="7a885-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="7a885-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a885-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a885-105">Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.</span><span class="sxs-lookup"><span data-stu-id="7a885-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="7a885-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a885-106">Properties</span></span>

| <span data-ttu-id="7a885-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a885-107">Property</span></span>     | <span data-ttu-id="7a885-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7a885-108">Type</span></span>        | <span data-ttu-id="7a885-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7a885-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a885-110">записей</span><span class="sxs-lookup"><span data-stu-id="7a885-110">credentials</span></span>|<span data-ttu-id="7a885-111">Коллекция [учетных данных](credential.md)</span><span class="sxs-lookup"><span data-stu-id="7a885-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="7a885-112">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="7a885-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="7a885-113">id</span><span class="sxs-lookup"><span data-stu-id="7a885-113">id</span></span>|<span data-ttu-id="7a885-114">String</span><span class="sxs-lookup"><span data-stu-id="7a885-114">String</span></span>|<span data-ttu-id="7a885-115">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="7a885-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a885-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a885-116">JSON representation</span></span>

<span data-ttu-id="7a885-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a885-117">The following is a JSON representation of the resource.</span></span>

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


