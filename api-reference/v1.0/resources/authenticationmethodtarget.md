---
title: тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f75a0ee81f1c43923a910bd86df4828c276706e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469110"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="d9de5-103">тип ресурса authenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="d9de5-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="d9de5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9de5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9de5-105">Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9de5-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="d9de5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9de5-106">Properties</span></span>
|<span data-ttu-id="d9de5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9de5-107">Property</span></span>|<span data-ttu-id="d9de5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d9de5-108">Type</span></span>|<span data-ttu-id="d9de5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d9de5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9de5-110">id</span><span class="sxs-lookup"><span data-stu-id="d9de5-110">id</span></span>|<span data-ttu-id="d9de5-111">String</span><span class="sxs-lookup"><span data-stu-id="d9de5-111">String</span></span>|<span data-ttu-id="d9de5-112">Объект Id пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9de5-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="d9de5-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="d9de5-113">isRegistrationRequired</span></span>|<span data-ttu-id="d9de5-114">Логический</span><span class="sxs-lookup"><span data-stu-id="d9de5-114">Boolean</span></span>|<span data-ttu-id="d9de5-115">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d9de5-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="d9de5-116">targetType</span><span class="sxs-lookup"><span data-stu-id="d9de5-116">targetType</span></span>|<span data-ttu-id="d9de5-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="d9de5-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="d9de5-118">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="d9de5-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="d9de5-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="d9de5-119">useForSignIn</span></span>|<span data-ttu-id="d9de5-120">Логический</span><span class="sxs-lookup"><span data-stu-id="d9de5-120">Boolean</span></span>|<span data-ttu-id="d9de5-121">Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9de5-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9de5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="d9de5-122">Relationships</span></span>
<span data-ttu-id="d9de5-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d9de5-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9de5-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d9de5-124">JSON representation</span></span>
<span data-ttu-id="d9de5-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9de5-125">The following is a JSON representation of the resource.</span></span>
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
