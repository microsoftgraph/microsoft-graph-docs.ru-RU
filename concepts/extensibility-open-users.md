---
title: Добавление пользовательских данных в ресурсы user с помощью открытых расширений
description: 'Мы рассмотрим пример использования *открытых расширений*. '
author: dkershaw10
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: c4039c1bb0e4972aa42ac9ee61c73095817b0368
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053790"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a><span data-ttu-id="6a8ef-103">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="6a8ef-103">Add custom data to users using open extensions</span></span>
<span data-ttu-id="6a8ef-104">Мы рассмотрим пример использования *открытых расширений*.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-104">We're going to walk you through an example to demonstrate how to use *open extensions*.</span></span> 

<span data-ttu-id="6a8ef-p101">Представьте, что вы разрабатываете приложение, доступное на множестве клиентских платформ, например на компьютерах и мобильных устройствах.  Вы хотите, чтобы пользователи могли настраивать интерфейс, чтобы он выглядел одинаково независимо от того, какое устройство они используют для входа в приложение. Это распространенное требование для приложений.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p101">Imagine you're building an application that is available on lots of different client platforms, such as desktop and mobile.  You want to let users configure their UI experience so it’s consistent no matter which device they use to sign in to your app. This is a common requirement for most apps.</span></span> 

<span data-ttu-id="6a8ef-108">В этой статье мы покажем вам, как:</span><span class="sxs-lookup"><span data-stu-id="6a8ef-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="6a8ef-109">добавить открытое расширение, представляющее данные перемещаемого профиля пользователя;</span><span class="sxs-lookup"><span data-stu-id="6a8ef-109">Add an open extension representing some roaming profile information about the user.</span></span>
2. <span data-ttu-id="6a8ef-110">запросить данные у пользователя и вернуть перемещаемый профиль;</span><span class="sxs-lookup"><span data-stu-id="6a8ef-110">Query the user and return the roaming profile.</span></span>
3. <span data-ttu-id="6a8ef-111">изменить данные перемещаемого профиля пользователя (значение открытого расширения);</span><span class="sxs-lookup"><span data-stu-id="6a8ef-111">Change the user's roaming profile information (the open extension value).</span></span>
4. <span data-ttu-id="6a8ef-112">удалить данные перемещаемого профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-112">Delete the user's roaming profile information.</span></span>

><span data-ttu-id="6a8ef-p102">**Примечание.** В этой статье показано, как добавлять, считывать, обновлять и удалять открытые расширения для ресурса *user*.  Эти методы также поддерживаются для типов ресурсов *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* и *organizaton*.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p102">**Note:** This topic shows you how to add, read, update and delete open extensions on a *user* resource.  These methods are also supported for the *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* and *organizaton* resource types.</span></span>  
<span data-ttu-id="6a8ef-p103">Просто измените приведенные ниже примеры запросов, используя любой из этих типов ресурсов. Приведенные ниже примеры можно сократить.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p103">Simply update the example requests below using any of those resource types. The responses shown in the examples below may be truncated for brevity.</span></span> 

## <a name="1-add-roaming-profile-information"></a><span data-ttu-id="6a8ef-117">1. Добавление данных перемещаемого профиля</span><span class="sxs-lookup"><span data-stu-id="6a8ef-117">1. Add roaming profile information</span></span>
<span data-ttu-id="6a8ef-p104">Пользователь входит в приложение и настраивает его внешний вид.  Эти параметры приложения должны перемещаться, чтобы интерфейс выглядел одинаково на любом устройстве.  В этой статье мы рассмотрим, как добавить данные перемещаемого профиля в ресурс пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p104">The user signs in to the app and configures the look and feel of the app.  These app settings should roam so that the user gets the same experience on whatever device they sign in to the app from.  Here we'll see how to add the roaming profile information to a user resource.</span></span>

##### <a name="request"></a><span data-ttu-id="6a8ef-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a8ef-121">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
##### <a name="response"></a><span data-ttu-id="6a8ef-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a8ef-122">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a><span data-ttu-id="6a8ef-123">2. Получение данных перемещаемого профиля</span><span class="sxs-lookup"><span data-stu-id="6a8ef-123">2. Retrieve roaming profile information</span></span>
<span data-ttu-id="6a8ef-p105">Когда пользователь входит в приложение с другого устройства, приложение может получить данные профиля пользователя, а также соответствующие параметры перемещения. Для этого можно получить ресурс пользователя и дополнить свойство навигации расширения.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p105">When the user signs in to the app from another device, the app can retrieve the user's profile details as well as their roaming settings. This can be done by getting the user's resource and expanding the extension navigation property.</span></span>

##### <a name="request"></a><span data-ttu-id="6a8ef-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a8ef-126">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
##### <a name="response"></a><span data-ttu-id="6a8ef-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a8ef-127">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
><span data-ttu-id="6a8ef-128">**Примечание.** Если у вас есть несколько расширений, вы можете отфильтровать их по свойству *id*, чтобы получить нужное расширение.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-128">**Note:** If you have multiple extensions, you can filter on the *id* to get the extension that you are interested in.</span></span>

## <a name="3-change-roaming-profile-information"></a><span data-ttu-id="6a8ef-129">3. Изменение данных перемещаемого профиля</span><span class="sxs-lookup"><span data-stu-id="6a8ef-129">3. Change roaming profile information</span></span>
<span data-ttu-id="6a8ef-p106">Пользователь может изменить данные своего перемещаемого профиля.  Это можно сделать с помощью запроса ```PATCH``` со значением открытого расширения.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p106">The user may choose to change their roaming profile information.  This update can be done with a ```PATCH``` on the open extension value.</span></span> 

##### <a name="request"></a><span data-ttu-id="6a8ef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a8ef-132">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

##### <a name="response"></a><span data-ttu-id="6a8ef-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a8ef-133">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a><span data-ttu-id="6a8ef-134">4. Удаление перемещаемого профиля пользователя</span><span class="sxs-lookup"><span data-stu-id="6a8ef-134">4. Delete a user's roaming profile</span></span>
<span data-ttu-id="6a8ef-p107">Пользователь решает, что ему не больше не нужен перемещаемый профиль, и удаляет его. Это можно сделать с помощью запроса ```DELETE``` со значением открытого расширения.</span><span class="sxs-lookup"><span data-stu-id="6a8ef-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>

##### <a name="request"></a><span data-ttu-id="6a8ef-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a8ef-137">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="6a8ef-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a8ef-138">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="6a8ef-139">См. также</span><span class="sxs-lookup"><span data-stu-id="6a8ef-139">See also</span></span>

- [<span data-ttu-id="6a8ef-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="6a8ef-140">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="6a8ef-141">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="6a8ef-141">Add custom data to groups using schema extensions</span></span>](extensibility-schema-groups.md)
- [<span data-ttu-id="6a8ef-142">Тип ресурса openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6a8ef-142">openTypeExtension resource type</span></span>](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="6a8ef-143">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="6a8ef-143">Create open extension</span></span>](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="6a8ef-144">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="6a8ef-144">Get open extension</span></span>](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="6a8ef-145">Обновление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="6a8ef-145">Update open extension</span></span>](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="6a8ef-146">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="6a8ef-146">Delete open extension</span></span>](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
