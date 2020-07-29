---
title: Получение Итеминсигхтс
description: Получение свойств объекта Итеминсигхтссеттингс
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 62c1a0f2efda751153d42d985d196a69e35caee5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509647"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="7529e-103">Получение Итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="7529e-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="7529e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7529e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7529e-105">Получение свойств объекта [итеминсигхтссеттингс](../resources/iteminsightssettings.md) .</span><span class="sxs-lookup"><span data-stu-id="7529e-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="7529e-106">Сведения о том, как настроить конфиденциальность сведений об элементах для вашей организации, можно узнать в разделе [Настройка конфиденциальности Insights](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="7529e-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="7529e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7529e-107">Permissions</span></span>

<span data-ttu-id="7529e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7529e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7529e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7529e-110">Permission type</span></span>      | <span data-ttu-id="7529e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7529e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7529e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7529e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7529e-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7529e-113">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="7529e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7529e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7529e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7529e-115">Not supported.</span></span>    |
|<span data-ttu-id="7529e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7529e-116">Application</span></span> | <span data-ttu-id="7529e-117">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7529e-117">User.Read, User.ReadWrite</span></span>  |

><span data-ttu-id="7529e-118">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="7529e-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="7529e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7529e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="7529e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7529e-120">Request headers</span></span>

| <span data-ttu-id="7529e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7529e-121">Name</span></span>       | <span data-ttu-id="7529e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7529e-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7529e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7529e-123">Authorization</span></span>  | <span data-ttu-id="7529e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7529e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7529e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7529e-126">Request body</span></span>

<span data-ttu-id="7529e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7529e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7529e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7529e-128">Response</span></span>

<span data-ttu-id="7529e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итеминсигхтссеттингс](../resources/iteminsightssettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7529e-129">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="7529e-130">**Примечание:** Эта операция проверяет допустимость значений свойств указанного ресурса **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="7529e-130">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="7529e-131">Если задано свойство **дисабледфорграуп** , эта операция не проверяет существование соответствующей группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7529e-131">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="7529e-132">Это означает, что если вы настроили **дисабледфорграуп** для группы Azure AD, которая не существовала или была удалена, то эта операция не сможет определить членство в группах и отключить сведения об элементе для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7529e-132">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="7529e-133">Если для параметра **исенаблединорганизатион** задано значение `true` , операция позволит получить информацию для всех пользователей в Организации.</span><span class="sxs-lookup"><span data-stu-id="7529e-133">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="7529e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7529e-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7529e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7529e-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7529e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7529e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="7529e-137">C#</span><span class="sxs-lookup"><span data-stu-id="7529e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7529e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7529e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7529e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7529e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7529e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7529e-140">Response</span></span>

<span data-ttu-id="7529e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7529e-141">Here is an example of the response.</span></span> 
> <span data-ttu-id="7529e-142">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="7529e-142">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7529e-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7529e-143">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "get_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
