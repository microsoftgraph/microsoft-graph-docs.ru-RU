---
title: Тип ресурса учетных данных
description: Указывает один учетный документ, используемый для входа в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0521f766a7a0da482cf67628c3816935ee9270b8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761683"
---
# <a name="credential-resource-type"></a><span data-ttu-id="8e259-103">Тип ресурса учетных данных</span><span class="sxs-lookup"><span data-stu-id="8e259-103">credential resource type</span></span>

<span data-ttu-id="8e259-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e259-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e259-105">Указывает один учетный документ, используемый для входа в приложение.</span><span class="sxs-lookup"><span data-stu-id="8e259-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="8e259-106">Например, имя пользователя — это один учетный данные, пароль — другой учетный данные.</span><span class="sxs-lookup"><span data-stu-id="8e259-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="8e259-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e259-107">Properties</span></span>

| <span data-ttu-id="8e259-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e259-108">Property</span></span>     | <span data-ttu-id="8e259-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8e259-109">Type</span></span>        | <span data-ttu-id="8e259-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8e259-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e259-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="8e259-111">fieldId</span></span>|<span data-ttu-id="8e259-112">String</span><span class="sxs-lookup"><span data-stu-id="8e259-112">String</span></span>|<span data-ttu-id="8e259-113">Имя поля для этого учетного данных.</span><span class="sxs-lookup"><span data-stu-id="8e259-113">The name of the field for this credential.</span></span> <span data-ttu-id="8e259-114">например, имя пользователя, пароль или phoneNumber.</span><span class="sxs-lookup"><span data-stu-id="8e259-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="8e259-115">Это определяется приложением.</span><span class="sxs-lookup"><span data-stu-id="8e259-115">This is defined by the application.</span></span> <span data-ttu-id="8e259-116">Должно совпадать с тем, что находится в html-поле на объекте singleSignOnSettings/password.</span><span class="sxs-lookup"><span data-stu-id="8e259-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="8e259-117">type</span><span class="sxs-lookup"><span data-stu-id="8e259-117">type</span></span>|<span data-ttu-id="8e259-118">String</span><span class="sxs-lookup"><span data-stu-id="8e259-118">String</span></span>|<span data-ttu-id="8e259-119">Тип для этого учетного данных.</span><span class="sxs-lookup"><span data-stu-id="8e259-119">The type for this credential.</span></span> <span data-ttu-id="8e259-120">Допустимые значения: имя пользователя, пароль или другие.</span><span class="sxs-lookup"><span data-stu-id="8e259-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="8e259-121">value</span><span class="sxs-lookup"><span data-stu-id="8e259-121">value</span></span>|<span data-ttu-id="8e259-122">String</span><span class="sxs-lookup"><span data-stu-id="8e259-122">String</span></span>|<span data-ttu-id="8e259-123">Значение для этого учетного данных.</span><span class="sxs-lookup"><span data-stu-id="8e259-123">The value for this credential.</span></span> <span data-ttu-id="8e259-124">например, mysuperhiddenpassword.</span><span class="sxs-lookup"><span data-stu-id="8e259-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="8e259-125">Обратите внимание, что значение для паролей является только для записи, значение никогда не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="8e259-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e259-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e259-126">JSON representation</span></span>

<span data-ttu-id="8e259-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e259-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


