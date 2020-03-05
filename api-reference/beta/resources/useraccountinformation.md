---
title: Тип ресурса Усераккаунтинформатион
description: Тип ресурса Усераккаунтинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cdeb6a676304fe4ec69207f9df6331d0df503b56
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519556"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="1f28a-103">Тип ресурса Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="1f28a-103">userAccountInformation resource type</span></span>

<span data-ttu-id="1f28a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f28a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f28a-105">Представляет сведения, специально связанные с учетной записью пользователя, будь то учетная запись Azure AD или учетная запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1f28a-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="1f28a-106">Идентификатор сущности задается соответствующим идентификаторам Azure AD AD или CID учетной записи Майкрософт соответственно.</span><span class="sxs-lookup"><span data-stu-id="1f28a-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="1f28a-107">Эти поля доступны только для чтения через Microsoft Graph и должны редактироваться с помощью профиля пользователя или администратора клиента для соответствующего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="1f28a-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="1f28a-108">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1f28a-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1f28a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1f28a-109">Methods</span></span>

| <span data-ttu-id="1f28a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1f28a-110">Method</span></span>                                                             | <span data-ttu-id="1f28a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f28a-111">Return Type</span></span>                                         | <span data-ttu-id="1f28a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1f28a-112">Description</span></span>                                                         |
|:-------------------------------------------------------------------|:----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="1f28a-113">Получение Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="1f28a-113">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md) | [<span data-ttu-id="1f28a-114">усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="1f28a-114">userAccountInformation</span></span>](useraccountinformation.md) | <span data-ttu-id="1f28a-115">Чтение свойств и связей объекта **усераккаунтинформатион** .</span><span class="sxs-lookup"><span data-stu-id="1f28a-115">Read the properties and relationships of a **userAccountInformation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f28a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f28a-116">Properties</span></span>

| <span data-ttu-id="1f28a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f28a-117">Property</span></span>            | <span data-ttu-id="1f28a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1f28a-118">Type</span></span>                       | <span data-ttu-id="1f28a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1f28a-119">Description</span></span>                                                                                                                              |
|:--------------------|:---------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1f28a-120">ageGroup</span><span class="sxs-lookup"><span data-stu-id="1f28a-120">ageGroup</span></span>             |<span data-ttu-id="1f28a-121">String</span><span class="sxs-lookup"><span data-stu-id="1f28a-121">String</span></span>                      | <span data-ttu-id="1f28a-122">Показывает группу возрастных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1f28a-122">Shows the age group of user.</span></span> <span data-ttu-id="1f28a-123">Допустимые `null`значения `minor`, `notAdult` и `adult` они создаются каталогом и не могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f28a-123">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="1f28a-124">countryCode</span><span class="sxs-lookup"><span data-stu-id="1f28a-124">countryCode</span></span>          |<span data-ttu-id="1f28a-125">String</span><span class="sxs-lookup"><span data-stu-id="1f28a-125">String</span></span>|                     | <span data-ttu-id="1f28a-126">Содержит двухбуквенный код страны, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f28a-126">Contains the two-character country code associated with the users account.</span></span>                                                                |
|<span data-ttu-id="1f28a-127">преферредлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="1f28a-127">preferredLanguageTag</span></span> |[<span data-ttu-id="1f28a-128">localeInfo</span><span class="sxs-lookup"><span data-stu-id="1f28a-128">localeInfo</span></span>](localeinfo.md) | <span data-ttu-id="1f28a-129">Содержит язык, который пользователь связал с учетной записью как предпочитаемый.</span><span class="sxs-lookup"><span data-stu-id="1f28a-129">Contains the language the user has associated as preferred for the account.</span></span>                                                              |
|<span data-ttu-id="1f28a-130">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f28a-130">userPrincipalName</span></span>    |<span data-ttu-id="1f28a-131">String</span><span class="sxs-lookup"><span data-stu-id="1f28a-131">String</span></span>                      | <span data-ttu-id="1f28a-132">Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="1f28a-132">The user principal name (UPN) of the user associated with the account.</span></span>                                                                   |

## <a name="relationships"></a><span data-ttu-id="1f28a-133">Связи</span><span class="sxs-lookup"><span data-stu-id="1f28a-133">Relationships</span></span>

<span data-ttu-id="1f28a-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1f28a-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f28a-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1f28a-135">JSON representation</span></span>

<span data-ttu-id="1f28a-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f28a-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": ""
}-->

```json
{
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {"@odata.type": "microsoft.graph.localeInfo"},
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAccountInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
