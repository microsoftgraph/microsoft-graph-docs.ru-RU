---
title: Тип ресурса Аусентикатионмесодтаржет
description: Коллекция пользователей или групп, которые включены для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7112249f618bbda31eddeb07967d201c8b641075
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418478"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="adfa6-103">Тип ресурса Аусентикатионмесодтаржет</span><span class="sxs-lookup"><span data-stu-id="adfa6-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="adfa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adfa6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adfa6-105">Коллекция пользователей или групп, которые включены для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="adfa6-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="adfa6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="adfa6-106">Properties</span></span>
|<span data-ttu-id="adfa6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="adfa6-107">Property</span></span>|<span data-ttu-id="adfa6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="adfa6-108">Type</span></span>|<span data-ttu-id="adfa6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="adfa6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adfa6-110">id</span><span class="sxs-lookup"><span data-stu-id="adfa6-110">id</span></span>|<span data-ttu-id="adfa6-111">String</span><span class="sxs-lookup"><span data-stu-id="adfa6-111">String</span></span>|<span data-ttu-id="adfa6-112">Идентификатор объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="adfa6-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="adfa6-113">исрегистратионрекуиред</span><span class="sxs-lookup"><span data-stu-id="adfa6-113">isRegistrationRequired</span></span>|<span data-ttu-id="adfa6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="adfa6-114">Boolean</span></span>|<span data-ttu-id="adfa6-115">Определяет, применяется ли пользователь для регистрации метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="adfa6-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="adfa6-116">targetType</span><span class="sxs-lookup"><span data-stu-id="adfa6-116">targetType</span></span>|<span data-ttu-id="adfa6-117">аусентикатионмесодтаржеттипе</span><span class="sxs-lookup"><span data-stu-id="adfa6-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="adfa6-118">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="adfa6-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="adfa6-119">усефорсигнин</span><span class="sxs-lookup"><span data-stu-id="adfa6-119">useForSignIn</span></span>|<span data-ttu-id="adfa6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="adfa6-120">Boolean</span></span>|<span data-ttu-id="adfa6-121">Определяет, можно ли использовать метод проверки подлинности для входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="adfa6-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adfa6-122">Связи</span><span class="sxs-lookup"><span data-stu-id="adfa6-122">Relationships</span></span>
<span data-ttu-id="adfa6-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="adfa6-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adfa6-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="adfa6-124">JSON representation</span></span>
<span data-ttu-id="adfa6-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adfa6-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
