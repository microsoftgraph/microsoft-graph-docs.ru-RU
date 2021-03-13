---
title: тип ресурса smsAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности текстовых сообщений.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4309316adfeff126f845dd362d5ffb8899a77e60
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761032"
---
# <a name="smsauthenticationmethodtarget-resource-type"></a><span data-ttu-id="02aa6-103">тип ресурса smsAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="02aa6-103">smsAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="02aa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02aa6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02aa6-105">Коллекция пользователей или групп, включенная для использования политики методов проверки [подлинности](../resources/smsAuthenticationMethodConfiguration.md) текстовых сообщений в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02aa6-105">A collection of users or groups enabled to use [Text Message authentication methods policy](../resources/smsAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="02aa6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="02aa6-106">Properties</span></span>
|<span data-ttu-id="02aa6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="02aa6-107">Property</span></span>|<span data-ttu-id="02aa6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="02aa6-108">Type</span></span>|<span data-ttu-id="02aa6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02aa6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02aa6-110">id</span><span class="sxs-lookup"><span data-stu-id="02aa6-110">id</span></span>|<span data-ttu-id="02aa6-111">String</span><span class="sxs-lookup"><span data-stu-id="02aa6-111">String</span></span>|<span data-ttu-id="02aa6-112">Объектный ID пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02aa6-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="02aa6-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="02aa6-113">isRegistrationRequired</span></span>|<span data-ttu-id="02aa6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="02aa6-114">Boolean</span></span>|<span data-ttu-id="02aa6-115">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="02aa6-115">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="02aa6-116">**Не поддерживается.**</span><span class="sxs-lookup"><span data-stu-id="02aa6-116">**Not supported**.</span></span>|
|<span data-ttu-id="02aa6-117">isUsableForSignIn</span><span class="sxs-lookup"><span data-stu-id="02aa6-117">isUsableForSignIn</span></span>|<span data-ttu-id="02aa6-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="02aa6-118">Boolean</span></span>|<span data-ttu-id="02aa6-119">Определяет, могут ли пользователи или группы использовать этот метод проверки подлинности для регистрации в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02aa6-119">Determines if the users or groups can use this authentication method to sign in to Azure AD.</span></span> <span data-ttu-id="02aa6-120">Значение всегда `true` .</span><span class="sxs-lookup"><span data-stu-id="02aa6-120">The value is always `true`.</span></span>|
|<span data-ttu-id="02aa6-121">targetType</span><span class="sxs-lookup"><span data-stu-id="02aa6-121">targetType</span></span>|<span data-ttu-id="02aa6-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="02aa6-122">authenticationMethodTargetType</span></span>| <span data-ttu-id="02aa6-123">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="02aa6-123">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02aa6-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="02aa6-124">Relationships</span></span>
<span data-ttu-id="02aa6-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="02aa6-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="02aa6-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="02aa6-126">JSON representation</span></span>
<span data-ttu-id="02aa6-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02aa6-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```
