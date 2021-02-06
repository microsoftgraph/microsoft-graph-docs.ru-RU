---
title: Тип ресурса passwordSingleSignOnCredentialSet
description: Указывает набор учетных данных, которые полностью определяют поток входа пользователя или группы в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 95526942bcedfc20d983a8873699af6902482b2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130886"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="416ee-103">Тип ресурса passwordSingleSignOnCredentialSet</span><span class="sxs-lookup"><span data-stu-id="416ee-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="416ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="416ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="416ee-105">Указывает набор учетных данных, которые полностью определяют поток входа пользователя или группы в приложение.</span><span class="sxs-lookup"><span data-stu-id="416ee-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="416ee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="416ee-106">Properties</span></span>

| <span data-ttu-id="416ee-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="416ee-107">Property</span></span>     | <span data-ttu-id="416ee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="416ee-108">Type</span></span>        | <span data-ttu-id="416ee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="416ee-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="416ee-110">credentials</span><span class="sxs-lookup"><span data-stu-id="416ee-110">credentials</span></span>|<span data-ttu-id="416ee-111">[коллекция учетных](credential.md) данных</span><span class="sxs-lookup"><span data-stu-id="416ee-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="416ee-112">Список объектов учетных данных, которые определяют полный поток входа.</span><span class="sxs-lookup"><span data-stu-id="416ee-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="416ee-113">id</span><span class="sxs-lookup"><span data-stu-id="416ee-113">id</span></span>|<span data-ttu-id="416ee-114">Строка</span><span class="sxs-lookup"><span data-stu-id="416ee-114">String</span></span>|<span data-ttu-id="416ee-115">ИД пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="416ee-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="416ee-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="416ee-116">JSON representation</span></span>

<span data-ttu-id="416ee-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="416ee-117">The following is a JSON representation of the resource.</span></span>

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


