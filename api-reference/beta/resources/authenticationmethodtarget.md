---
title: Тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать метод проверки подлинности в рамках политики методов проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 19f8fb774ad0a60fa74d2c27655ee1174e0989af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135452"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="97546-103">Тип ресурса authenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="97546-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="97546-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97546-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97546-105">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности в рамках политики методов проверки подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="97546-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="97546-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97546-106">Properties</span></span>
|<span data-ttu-id="97546-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="97546-107">Property</span></span>|<span data-ttu-id="97546-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97546-108">Type</span></span>|<span data-ttu-id="97546-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97546-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97546-110">id</span><span class="sxs-lookup"><span data-stu-id="97546-110">id</span></span>|<span data-ttu-id="97546-111">Строка</span><span class="sxs-lookup"><span data-stu-id="97546-111">String</span></span>|<span data-ttu-id="97546-112">ИД объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="97546-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="97546-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="97546-113">isRegistrationRequired</span></span>|<span data-ttu-id="97546-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="97546-114">Boolean</span></span>|<span data-ttu-id="97546-115">Определяет, принудительно ли зарегистрирует метод проверки подлинности для пользователя.</span><span class="sxs-lookup"><span data-stu-id="97546-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="97546-116">targetType</span><span class="sxs-lookup"><span data-stu-id="97546-116">targetType</span></span>|<span data-ttu-id="97546-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="97546-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="97546-118">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="97546-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="97546-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="97546-119">useForSignIn</span></span>|<span data-ttu-id="97546-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="97546-120">Boolean</span></span>|<span data-ttu-id="97546-121">Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="97546-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97546-122">Связи</span><span class="sxs-lookup"><span data-stu-id="97546-122">Relationships</span></span>
<span data-ttu-id="97546-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97546-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97546-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97546-124">JSON representation</span></span>
<span data-ttu-id="97546-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97546-125">The following is a JSON representation of the resource.</span></span>
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
