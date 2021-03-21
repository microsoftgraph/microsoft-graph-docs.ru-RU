---
title: тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c9265fa359e5b60da6f8e36c13d1a4340ba6d1a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964983"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="bf779-103">тип ресурса authenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="bf779-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="bf779-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf779-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf779-105">Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf779-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="bf779-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf779-106">Properties</span></span>
|<span data-ttu-id="bf779-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf779-107">Property</span></span>|<span data-ttu-id="bf779-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bf779-108">Type</span></span>|<span data-ttu-id="bf779-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bf779-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf779-110">id</span><span class="sxs-lookup"><span data-stu-id="bf779-110">id</span></span>|<span data-ttu-id="bf779-111">String</span><span class="sxs-lookup"><span data-stu-id="bf779-111">String</span></span>|<span data-ttu-id="bf779-112">Объект Id пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf779-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="bf779-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="bf779-113">isRegistrationRequired</span></span>|<span data-ttu-id="bf779-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf779-114">Boolean</span></span>|<span data-ttu-id="bf779-115">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bf779-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="bf779-116">targetType</span><span class="sxs-lookup"><span data-stu-id="bf779-116">targetType</span></span>|<span data-ttu-id="bf779-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="bf779-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="bf779-118">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="bf779-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="bf779-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="bf779-119">useForSignIn</span></span>|<span data-ttu-id="bf779-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf779-120">Boolean</span></span>|<span data-ttu-id="bf779-121">Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf779-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf779-122">Связи</span><span class="sxs-lookup"><span data-stu-id="bf779-122">Relationships</span></span>
<span data-ttu-id="bf779-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bf779-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf779-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bf779-124">JSON representation</span></span>
<span data-ttu-id="bf779-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf779-125">The following is a JSON representation of the resource.</span></span>
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
