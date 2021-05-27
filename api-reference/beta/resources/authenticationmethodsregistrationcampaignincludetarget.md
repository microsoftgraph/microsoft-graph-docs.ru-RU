---
title: тип ресурса authenticationMethodsRegistrationCampaignIncludeTarget
description: Разрешить пользователям и группам пользователей настроить целевые методы проверки подлинности.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04dc753dd1a574bbf0b30d29b4b80375e7ab9a2c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682930"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a><span data-ttu-id="07f4d-103">тип ресурса authenticationMethodsRegistrationCampaignIncludeTarget</span><span class="sxs-lookup"><span data-stu-id="07f4d-103">authenticationMethodsRegistrationCampaignIncludeTarget resource type</span></span>

<span data-ttu-id="07f4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07f4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07f4d-105">Представляет пользователей и группы, которые ориентированы на кампании по регистрации метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="07f4d-105">Represents the users and groups that are targeted for authentication method registration campaigns.</span></span> <span data-ttu-id="07f4d-106">Целевыми являются только пользователи и группы, которые могут настроить метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="07f4d-106">Only users and groups that are enabled by the policy to set up the authentication method are targeted.</span></span>

## <a name="properties"></a><span data-ttu-id="07f4d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="07f4d-107">Properties</span></span>
|<span data-ttu-id="07f4d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="07f4d-108">Property</span></span>|<span data-ttu-id="07f4d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="07f4d-109">Type</span></span>|<span data-ttu-id="07f4d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07f4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f4d-111">id</span><span class="sxs-lookup"><span data-stu-id="07f4d-111">id</span></span>|<span data-ttu-id="07f4d-112">String</span><span class="sxs-lookup"><span data-stu-id="07f4d-112">String</span></span>|<span data-ttu-id="07f4d-113">Идентификатор объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="07f4d-113">The object identifier of an Azure AD user or group.</span></span>|
|<span data-ttu-id="07f4d-114">targetedAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="07f4d-114">targetedAuthenticationMethod</span></span>|<span data-ttu-id="07f4d-115">String</span><span class="sxs-lookup"><span data-stu-id="07f4d-115">String</span></span>|<span data-ttu-id="07f4d-116">Метод проверки подлинности, который пользователю предложено зарегистрировать.</span><span class="sxs-lookup"><span data-stu-id="07f4d-116">The authentication method that the user is prompted to register.</span></span> <span data-ttu-id="07f4d-117">Значение должно быть `microsoftAuthenticator` .</span><span class="sxs-lookup"><span data-stu-id="07f4d-117">The value must be `microsoftAuthenticator`.</span></span>|
|<span data-ttu-id="07f4d-118">targetType</span><span class="sxs-lookup"><span data-stu-id="07f4d-118">targetType</span></span>|<span data-ttu-id="07f4d-119">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="07f4d-119">authenticationMethodTargetType</span></span>|<span data-ttu-id="07f4d-120">Тип целевой цели метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="07f4d-120">The type of the authentication method target.</span></span> <span data-ttu-id="07f4d-121">Возможные значения: `user`, `group`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="07f4d-121">Possible values are: `user`, `group`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07f4d-122">Связи</span><span class="sxs-lookup"><span data-stu-id="07f4d-122">Relationships</span></span>
<span data-ttu-id="07f4d-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="07f4d-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07f4d-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="07f4d-124">JSON representation</span></span>
<span data-ttu-id="07f4d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07f4d-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "targetedAuthenticationMethod": "String"
}
```
