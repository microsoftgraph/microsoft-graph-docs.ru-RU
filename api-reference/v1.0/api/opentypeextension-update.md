---
title: Обновление открытого расширения
description: 'Обновление открытого расширения (объекта openTypeExtension) с использованием свойств, указанных в теле запроса:'
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 89804b1259f3832b2b69e2f62d25ac1fa8856809
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863693"
---
# <a name="update-open-extension"></a><span data-ttu-id="18be4-103">Обновление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="18be4-103">Update open extension</span></span>

<span data-ttu-id="18be4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18be4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18be4-105">Обновление открытого расширения (объекта[openTypeExtension](../resources/opentypeextension.md) ) с использованием свойств, указанных в теле запроса:</span><span class="sxs-lookup"><span data-stu-id="18be4-105">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="18be4-106">Если свойство в теле запроса совпадает с именем существующего свойства в расширении, то данные в расширении будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="18be4-106">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="18be4-107">В противном случае это свойство и его данные будут добавлены в расширение.</span><span class="sxs-lookup"><span data-stu-id="18be4-107">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="18be4-108">Данные в расширении могут относиться к элементарным типам или массиву элементарных типов.</span><span class="sxs-lookup"><span data-stu-id="18be4-108">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="18be4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18be4-109">Permissions</span></span>

<span data-ttu-id="18be4-110">В зависимости от ресурса, в котором было создано расширение, и запрошенного типа разрешений (делегированного или приложения), разрешение, указанное в следующей таблице, является минимальным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="18be4-110">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="18be4-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18be4-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18be4-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="18be4-112">Supported resource</span></span> | <span data-ttu-id="18be4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18be4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18be4-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18be4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18be4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18be4-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="18be4-116">device</span><span class="sxs-lookup"><span data-stu-id="18be4-116">device</span></span>](../resources/device.md) | <span data-ttu-id="18be4-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18be4-117">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="18be4-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="18be4-118">Not supported</span></span> | <span data-ttu-id="18be4-119">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-119">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="18be4-120">event</span><span class="sxs-lookup"><span data-stu-id="18be4-120">event</span></span>](../resources/event.md) | <span data-ttu-id="18be4-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="18be4-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="18be4-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-123">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="18be4-124">group</span><span class="sxs-lookup"><span data-stu-id="18be4-124">group</span></span>](../resources/group.md) | <span data-ttu-id="18be4-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="18be4-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="18be4-126">Not supported</span></span> | <span data-ttu-id="18be4-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-127">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="18be4-128">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="18be4-128">[group event](../resources/event.md)</span></span> | <span data-ttu-id="18be4-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="18be4-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="18be4-130">Not supported</span></span> | <span data-ttu-id="18be4-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="18be4-131">Not supported</span></span> |
| <span data-ttu-id="18be4-132">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="18be4-132">[group post](../resources/post.md)</span></span> | <span data-ttu-id="18be4-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-133">Group.ReadWrite.All</span></span> | <span data-ttu-id="18be4-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="18be4-134">Not supported</span></span> | <span data-ttu-id="18be4-135">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-135">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="18be4-136">message</span><span class="sxs-lookup"><span data-stu-id="18be4-136">message</span></span>](../resources/message.md) | <span data-ttu-id="18be4-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-137">Mail.ReadWrite</span></span> | <span data-ttu-id="18be4-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-138">Mail.ReadWrite</span></span> | <span data-ttu-id="18be4-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-139">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="18be4-140">organization</span><span class="sxs-lookup"><span data-stu-id="18be4-140">organization</span></span>](../resources/organization.md) | <span data-ttu-id="18be4-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-141">Organization.ReadWrite.All</span></span> | <span data-ttu-id="18be4-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="18be4-142">Not supported</span></span> | <span data-ttu-id="18be4-143">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-143">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="18be4-144">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="18be4-144">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="18be4-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="18be4-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="18be4-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-147">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="18be4-148">user</span><span class="sxs-lookup"><span data-stu-id="18be4-148">user</span></span>](../resources/user.md) | <span data-ttu-id="18be4-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-149">User.ReadWrite</span></span> | <span data-ttu-id="18be4-150">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18be4-150">User.ReadWrite</span></span> | <span data-ttu-id="18be4-151">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18be4-151">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18be4-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18be4-152">HTTP request</span></span>
<span data-ttu-id="18be4-153">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `PATCH` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="18be4-153">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

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
```

><span data-ttu-id="18be4-154">**Примечание:** Приведенный выше синтаксис показывает некоторые распространенные способы идентификации экземпляра ресурса, чтобы обновить добавочный номер.</span><span class="sxs-lookup"><span data-stu-id="18be4-154">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it.</span></span> <span data-ttu-id="18be4-155">Весь другой синтаксис, позволяющий определить эти экземпляры ресурса, поддерживает обновление открытых расширений в них подобным образом.</span><span class="sxs-lookup"><span data-stu-id="18be4-155">All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="18be4-156">См. раздел [Тело запроса](#request-body) о том, как включить в тело запроса специальные данные для изменения или дополнения этого расширения.</span><span class="sxs-lookup"><span data-stu-id="18be4-156">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="18be4-157">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="18be4-157">Path parameters</span></span>
|<span data-ttu-id="18be4-158">Параметр</span><span class="sxs-lookup"><span data-stu-id="18be4-158">Parameter</span></span>|<span data-ttu-id="18be4-159">Тип</span><span class="sxs-lookup"><span data-stu-id="18be4-159">Type</span></span>|<span data-ttu-id="18be4-160">Описание</span><span class="sxs-lookup"><span data-stu-id="18be4-160">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="18be4-161">id</span><span class="sxs-lookup"><span data-stu-id="18be4-161">id</span></span>|<span data-ttu-id="18be4-162">строка</span><span class="sxs-lookup"><span data-stu-id="18be4-162">string</span></span>|<span data-ttu-id="18be4-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18be4-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="18be4-165">extensionId</span><span class="sxs-lookup"><span data-stu-id="18be4-165">extensionId</span></span>|<span data-ttu-id="18be4-166">string</span><span class="sxs-lookup"><span data-stu-id="18be4-166">string</span></span>|<span data-ttu-id="18be4-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18be4-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="18be4-170">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18be4-170">Request headers</span></span>
| <span data-ttu-id="18be4-171">Имя</span><span class="sxs-lookup"><span data-stu-id="18be4-171">Name</span></span>       | <span data-ttu-id="18be4-172">Значение</span><span class="sxs-lookup"><span data-stu-id="18be4-172">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="18be4-173">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18be4-173">Authorization</span></span> | <span data-ttu-id="18be4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18be4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18be4-176">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18be4-176">Content-Type</span></span> | <span data-ttu-id="18be4-177">application/json</span><span class="sxs-lookup"><span data-stu-id="18be4-177">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="18be4-178">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18be4-178">Request body</span></span>

<span data-ttu-id="18be4-p106">Задайте основной текст JSON объекта [openTypeExtension](../resources/opentypeextension.md) с указанными ниже обязательными парами имя-значение и любыми пользовательскими данными, которые необходимо изменить или добавить в это расширение. Полезные данные JSON могут иметь простой тип или представлять собой массив элементов простого типа.</span><span class="sxs-lookup"><span data-stu-id="18be4-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="18be4-181">Имя</span><span class="sxs-lookup"><span data-stu-id="18be4-181">Name</span></span>       | <span data-ttu-id="18be4-182">Значение</span><span class="sxs-lookup"><span data-stu-id="18be4-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="18be4-183">@odata.type</span><span class="sxs-lookup"><span data-stu-id="18be4-183">@odata.type</span></span> | <span data-ttu-id="18be4-184">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="18be4-184">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="18be4-185">extensionName</span><span class="sxs-lookup"><span data-stu-id="18be4-185">extensionName</span></span> | <span data-ttu-id="18be4-186">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="18be4-186">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="18be4-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="18be4-187">Response</span></span>

<span data-ttu-id="18be4-188">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [openTypeExtension](../resources/opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="18be4-188">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="18be4-189">Пример</span><span class="sxs-lookup"><span data-stu-id="18be4-189">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="18be4-190">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="18be4-190">Request 1</span></span>

<span data-ttu-id="18be4-p107">В первом примере показано, как обновить расширение в сообщении. Изначально расширение представлено указанными ниже полезными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="18be4-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

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

<span data-ttu-id="18be4-193">Вы можете ссылаться на расширение по его имени:</span><span class="sxs-lookup"><span data-stu-id="18be4-193">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="18be4-194">Кроме того, вы можете ссылаться на расширение по его полному имени:</span><span class="sxs-lookup"><span data-stu-id="18be4-194">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="18be4-195">Для обновления указанного выше расширения используйте любой пример запроса и приведенный ниже тело запроса следующими способами:</span><span class="sxs-lookup"><span data-stu-id="18be4-195">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="18be4-196">изменив значение параметра `companyName` с `Wingtip Toys` на `Wingtip Toys (USA)`;</span><span class="sxs-lookup"><span data-stu-id="18be4-196">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="18be4-197">изменив значение параметра `dealValue` с `500050` на `500100`;</span><span class="sxs-lookup"><span data-stu-id="18be4-197">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="18be4-198">добавив новые данные в качестве пользовательского свойства `updated`.</span><span class="sxs-lookup"><span data-stu-id="18be4-198">Adding new data as the custom property `updated`</span></span>

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


#### <a name="response-1"></a><span data-ttu-id="18be4-199">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="18be4-199">Response 1</span></span>

<span data-ttu-id="18be4-200">Вот отклик, который не зависит от способа, которым вы ссылаетесь на расширение.</span><span class="sxs-lookup"><span data-stu-id="18be4-200">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="18be4-201">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="18be4-201">Request 2</span></span>

<span data-ttu-id="18be4-p108">Во втором примере показано, как обновить расширение в публикации группы. Изначально расширение представлено указанными ниже полезными данными JSON, в котором параметр `expirationDate` имеет значение `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="18be4-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

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

<span data-ttu-id="18be4-204">Ниже приведен запрос и тело запроса для изменения значения параметра `expirationDate` на `2016-07-30T11:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="18be4-204">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

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

#### <a name="response-2"></a><span data-ttu-id="18be4-205">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="18be4-205">Response 2</span></span>

<span data-ttu-id="18be4-206">Вот отклик для второго примера, в котором отображается обновленный параметр `expirationDate` в расширении.</span><span class="sxs-lookup"><span data-stu-id="18be4-206">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

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
