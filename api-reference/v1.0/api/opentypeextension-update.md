---
title: Обновление открытого расширения
description: 'Обновление открытого расширения (объекта openTypeExtension) со свойствами в теле запроса:'
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 87a56bd0728f069748da23edfbf71f8ebd1dec76
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092444"
---
# <a name="update-open-extension"></a><span data-ttu-id="43a86-103">Обновление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="43a86-103">Update open extension</span></span>

<span data-ttu-id="43a86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43a86-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43a86-105">Обновление открытого расширения[(объекта openTypeExtension)](../resources/opentypeextension.md) со свойствами в теле запроса:</span><span class="sxs-lookup"><span data-stu-id="43a86-105">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="43a86-106">Если свойство в теле запроса совпадает с именем существующего свойства в расширении, то данные в расширении будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="43a86-106">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="43a86-107">В противном случае это свойство и его данные будут добавлены в расширение.</span><span class="sxs-lookup"><span data-stu-id="43a86-107">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="43a86-108">Данные в расширении могут относиться к элементарным типам или массиву элементарных типов.</span><span class="sxs-lookup"><span data-stu-id="43a86-108">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

<span data-ttu-id="43a86-109">Список ресурсов, [](#permissions) которые поддерживают открытые расширения, см. в таблице в разделе "Разрешения".</span><span class="sxs-lookup"><span data-stu-id="43a86-109">See the table in the [Permissions](#permissions) section for the list of resources that support open extensions.</span></span>

## <a name="permissions"></a><span data-ttu-id="43a86-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43a86-110">Permissions</span></span>

<span data-ttu-id="43a86-111">В зависимости от ресурса, в который было создано расширение, и запрашиваемого типа разрешений (делегирование или приложение), разрешение, указанное в следующей таблице, является наименее привилегированным для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="43a86-111">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="43a86-112">Чтобы узнать больше, в том [числе](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) с осторожностью перед выбором более привилегированных разрешений, найди следующие разрешения в [разрешениях.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="43a86-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43a86-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="43a86-113">Supported resource</span></span> | <span data-ttu-id="43a86-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43a86-114">Delegated (work or school account)</span></span> | <span data-ttu-id="43a86-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43a86-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43a86-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43a86-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="43a86-117">device</span><span class="sxs-lookup"><span data-stu-id="43a86-117">device</span></span>](../resources/device.md) | <span data-ttu-id="43a86-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43a86-118">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="43a86-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="43a86-119">Not supported</span></span> | <span data-ttu-id="43a86-120">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-120">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="43a86-121">event</span><span class="sxs-lookup"><span data-stu-id="43a86-121">event</span></span>](../resources/event.md) | <span data-ttu-id="43a86-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="43a86-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="43a86-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-124">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="43a86-125">group</span><span class="sxs-lookup"><span data-stu-id="43a86-125">group</span></span>](../resources/group.md) | <span data-ttu-id="43a86-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="43a86-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="43a86-127">Not supported</span></span> | <span data-ttu-id="43a86-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-128">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="43a86-129">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="43a86-129">[group event](../resources/event.md)</span></span> | <span data-ttu-id="43a86-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="43a86-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="43a86-131">Not supported</span></span> | <span data-ttu-id="43a86-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="43a86-132">Not supported</span></span> |
| <span data-ttu-id="43a86-133">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="43a86-133">[group post](../resources/post.md)</span></span> | <span data-ttu-id="43a86-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-134">Group.ReadWrite.All</span></span> | <span data-ttu-id="43a86-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="43a86-135">Not supported</span></span> | <span data-ttu-id="43a86-136">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-136">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="43a86-137">message</span><span class="sxs-lookup"><span data-stu-id="43a86-137">message</span></span>](../resources/message.md) | <span data-ttu-id="43a86-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-138">Mail.ReadWrite</span></span> | <span data-ttu-id="43a86-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-139">Mail.ReadWrite</span></span> | <span data-ttu-id="43a86-140">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-140">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="43a86-141">organization</span><span class="sxs-lookup"><span data-stu-id="43a86-141">organization</span></span>](../resources/organization.md) | <span data-ttu-id="43a86-142">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-142">Organization.ReadWrite.All</span></span> | <span data-ttu-id="43a86-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="43a86-143">Not supported</span></span> | <span data-ttu-id="43a86-144">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-144">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="43a86-145">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="43a86-145">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="43a86-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="43a86-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-147">Contacts.ReadWrite</span></span> | <span data-ttu-id="43a86-148">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-148">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="43a86-149">user</span><span class="sxs-lookup"><span data-stu-id="43a86-149">user</span></span>](../resources/user.md) | <span data-ttu-id="43a86-150">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-150">User.ReadWrite</span></span> | <span data-ttu-id="43a86-151">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-151">User.ReadWrite</span></span> | <span data-ttu-id="43a86-152">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-152">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="43a86-153">task</span><span class="sxs-lookup"><span data-stu-id="43a86-153">task</span></span>](../resources/todotask.md) | <span data-ttu-id="43a86-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-154">Tasks.ReadWrite</span></span> | <span data-ttu-id="43a86-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="43a86-156">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-156">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="43a86-157">tasklist</span><span class="sxs-lookup"><span data-stu-id="43a86-157">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="43a86-158">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-158">Tasks.ReadWrite</span></span> | <span data-ttu-id="43a86-159">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43a86-159">Tasks.ReadWrite</span></span> | <span data-ttu-id="43a86-160">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a86-160">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43a86-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43a86-161">HTTP request</span></span>
<span data-ttu-id="43a86-162">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `PATCH` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="43a86-162">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
PATCH /users/me/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
PATCH /users/me/todo/lists/{todoTaskListId}/extensions/{extensionId}
```

><span data-ttu-id="43a86-163">**Примечание.** В примере выше показаны некоторые распространенные способы идентификации экземпляра ресурса для обновления расширения в нем.</span><span class="sxs-lookup"><span data-stu-id="43a86-163">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="43a86-164">Весь другой синтаксис, позволяющий идентифицировать эти экземпляры ресурсов, поддерживает обновление открытых расширений в них аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="43a86-164">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="43a86-165">См. раздел [Тело запроса](#request-body) о том, как включить в тело запроса специальные данные для изменения или дополнения этого расширения.</span><span class="sxs-lookup"><span data-stu-id="43a86-165">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="43a86-166">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="43a86-166">Path parameters</span></span>
|<span data-ttu-id="43a86-167">Параметр</span><span class="sxs-lookup"><span data-stu-id="43a86-167">Parameter</span></span>|<span data-ttu-id="43a86-168">Тип</span><span class="sxs-lookup"><span data-stu-id="43a86-168">Type</span></span>|<span data-ttu-id="43a86-169">Описание</span><span class="sxs-lookup"><span data-stu-id="43a86-169">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="43a86-170">id</span><span class="sxs-lookup"><span data-stu-id="43a86-170">id</span></span>|<span data-ttu-id="43a86-171">string</span><span class="sxs-lookup"><span data-stu-id="43a86-171">string</span></span>|<span data-ttu-id="43a86-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43a86-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="43a86-174">extensionId</span><span class="sxs-lookup"><span data-stu-id="43a86-174">extensionId</span></span>|<span data-ttu-id="43a86-175">string</span><span class="sxs-lookup"><span data-stu-id="43a86-175">string</span></span>|<span data-ttu-id="43a86-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43a86-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="43a86-179">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43a86-179">Request headers</span></span>
| <span data-ttu-id="43a86-180">Имя</span><span class="sxs-lookup"><span data-stu-id="43a86-180">Name</span></span>       | <span data-ttu-id="43a86-181">Значение</span><span class="sxs-lookup"><span data-stu-id="43a86-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="43a86-182">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43a86-182">Authorization</span></span> | <span data-ttu-id="43a86-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43a86-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43a86-185">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43a86-185">Content-Type</span></span> | <span data-ttu-id="43a86-186">application/json</span><span class="sxs-lookup"><span data-stu-id="43a86-186">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="43a86-187">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43a86-187">Request body</span></span>

<span data-ttu-id="43a86-p106">Задайте основной текст JSON объекта [openTypeExtension](../resources/opentypeextension.md) с указанными ниже обязательными парами имя-значение и любыми пользовательскими данными, которые необходимо изменить или добавить в это расширение. Полезные данные JSON могут иметь простой тип или представлять собой массив элементов простого типа.</span><span class="sxs-lookup"><span data-stu-id="43a86-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="43a86-190">Имя</span><span class="sxs-lookup"><span data-stu-id="43a86-190">Name</span></span>       | <span data-ttu-id="43a86-191">Значение</span><span class="sxs-lookup"><span data-stu-id="43a86-191">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="43a86-192">@odata.type</span><span class="sxs-lookup"><span data-stu-id="43a86-192">@odata.type</span></span> | <span data-ttu-id="43a86-193">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="43a86-193">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="43a86-194">extensionName</span><span class="sxs-lookup"><span data-stu-id="43a86-194">extensionName</span></span> | <span data-ttu-id="43a86-195">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="43a86-195">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="43a86-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="43a86-196">Response</span></span>

<span data-ttu-id="43a86-197">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="43a86-197">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="43a86-198">Пример</span><span class="sxs-lookup"><span data-stu-id="43a86-198">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="43a86-199">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="43a86-199">Request 1</span></span>

<span data-ttu-id="43a86-p107">В первом примере показано, как обновить расширение в сообщении. Изначально расширение представлено указанными ниже полезными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="43a86-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="43a86-202">Вы можете ссылаться на расширение по его имени:</span><span class="sxs-lookup"><span data-stu-id="43a86-202">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="43a86-203">Кроме того, вы можете ссылаться на расширение по его полному имени:</span><span class="sxs-lookup"><span data-stu-id="43a86-203">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="43a86-204">Для обновления указанного выше расширения используйте любой пример запроса и приведенный ниже тело запроса следующими способами:</span><span class="sxs-lookup"><span data-stu-id="43a86-204">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="43a86-205">изменив значение параметра `companyName` с `Wingtip Toys` на `Wingtip Toys (USA)`;</span><span class="sxs-lookup"><span data-stu-id="43a86-205">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="43a86-206">изменив значение параметра `dealValue` с `500050` на `500100`;</span><span class="sxs-lookup"><span data-stu-id="43a86-206">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="43a86-207">добавив новые данные в качестве пользовательского свойства `updated`.</span><span class="sxs-lookup"><span data-stu-id="43a86-207">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="43a86-208">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="43a86-208">Response 1</span></span>

<span data-ttu-id="43a86-209">Вот отклик, который не зависит от способа, которым вы ссылаетесь на расширение.</span><span class="sxs-lookup"><span data-stu-id="43a86-209">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="43a86-210">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="43a86-210">Request 2</span></span>

<span data-ttu-id="43a86-p108">Во втором примере показано, как обновить расширение в публикации группы. Изначально расширение представлено указанными ниже полезными данными JSON, в котором параметр `expirationDate` имеет значение `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="43a86-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="43a86-213">Ниже приведен запрос и тело запроса для изменения значения параметра `expirationDate` на `2016-07-30T11:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="43a86-213">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"],
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="43a86-214">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="43a86-214">Response 2</span></span>

<span data-ttu-id="43a86-215">Вот отклик для второго примера, в котором отображается обновленный параметр `expirationDate` в расширении.</span><span class="sxs-lookup"><span data-stu-id="43a86-215">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "ignored",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->

