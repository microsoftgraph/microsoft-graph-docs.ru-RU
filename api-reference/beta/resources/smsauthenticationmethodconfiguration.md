---
title: тип ресурса smsAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности текстовых сообщений.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5a5e62e17e5b2e1cbc96ed96a44a0c483db981d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761039"
---
# <a name="smsauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="b8260-103">тип ресурса smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8260-103">smsAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="b8260-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8260-105">Представляет политику методов проверки подлинности текстовых сообщений.</span><span class="sxs-lookup"><span data-stu-id="b8260-105">Represents a Text Message authentication methods policy.</span></span> <span data-ttu-id="b8260-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b8260-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="b8260-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b8260-107">Methods</span></span>
|<span data-ttu-id="b8260-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b8260-108">Method</span></span>|<span data-ttu-id="b8260-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="b8260-109">Return type</span></span>|<span data-ttu-id="b8260-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8260-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8260-111">[получение](../api/smsauthenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="b8260-111">[Get](../api/smsauthenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="b8260-112">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8260-112">smsAuthenticationMethodConfiguration</span></span>](../resources/smsauthenticationmethodconfiguration.md)|<span data-ttu-id="b8260-113">Ознакомьтесь с свойствами и отношениями объекта smsAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b8260-113">Read the properties and relationships of a smsAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="b8260-114">Update</span><span class="sxs-lookup"><span data-stu-id="b8260-114">Update</span></span>](../api/smsauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="b8260-115">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8260-115">smsAuthenticationMethodConfiguration</span></span>](../resources/smsauthenticationmethodconfiguration.md)|<span data-ttu-id="b8260-116">Обновление свойств объекта smsAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b8260-116">Update the properties of a smsAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="b8260-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="b8260-117">Delete</span></span>](../api/smsauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="b8260-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b8260-118">None</span></span>|<span data-ttu-id="b8260-119">Возвращает объект smsAuthenticationMethodConfiguration к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b8260-119">Reverts the smsAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8260-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8260-120">Properties</span></span>
|<span data-ttu-id="b8260-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8260-121">Property</span></span>|<span data-ttu-id="b8260-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b8260-122">Type</span></span>|<span data-ttu-id="b8260-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b8260-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8260-124">id</span><span class="sxs-lookup"><span data-stu-id="b8260-124">id</span></span>|<span data-ttu-id="b8260-125">String</span><span class="sxs-lookup"><span data-stu-id="b8260-125">String</span></span>|<span data-ttu-id="b8260-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b8260-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="b8260-127">state</span><span class="sxs-lookup"><span data-stu-id="b8260-127">state</span></span>|<span data-ttu-id="b8260-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="b8260-128">authenticationMethodState</span></span>|<span data-ttu-id="b8260-129">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b8260-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8260-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="b8260-130">Relationships</span></span>
|<span data-ttu-id="b8260-131">Связь</span><span class="sxs-lookup"><span data-stu-id="b8260-131">Relationship</span></span>|<span data-ttu-id="b8260-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b8260-132">Type</span></span>|<span data-ttu-id="b8260-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b8260-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8260-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="b8260-134">includeTargets</span></span>|<span data-ttu-id="b8260-135">[коллекция smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="b8260-135">[smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="b8260-136">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b8260-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8260-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8260-137">JSON representation</span></span>
<span data-ttu-id="b8260-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8260-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

