---
title: Get itemInsights
description: Извлечение свойств объекта itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 3e8af098035d89dbcea3436c0a17721c4d9dfc48
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443862"
---
# <a name="get-iteminsightssettings"></a><span data-ttu-id="4a11e-103">Get itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="4a11e-103">Get itemInsightsSettings</span></span>

<span data-ttu-id="4a11e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a11e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a11e-105">Получите свойства [объекта itemInsightsSettings.](../resources/iteminsightssettings.md)</span><span class="sxs-lookup"><span data-stu-id="4a11e-105">Get the properties of [itemInsightsSettings](../resources/iteminsightssettings.md) object.</span></span>

<span data-ttu-id="4a11e-106">Сведения о настройке конфиденциальности элементов для организации см. в статье [Настройка конфиденциальности .](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="4a11e-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4a11e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a11e-107">Permissions</span></span>

<span data-ttu-id="4a11e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a11e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a11e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a11e-110">Permission type</span></span>      | <span data-ttu-id="4a11e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a11e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a11e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a11e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a11e-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a11e-113">User.Read.All, User.ReadWrite.All</span></span> |
|<span data-ttu-id="4a11e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a11e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a11e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a11e-115">Not supported.</span></span>    |
|<span data-ttu-id="4a11e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a11e-116">Application</span></span> | <span data-ttu-id="4a11e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a11e-117">Not supported.</span></span> |

><span data-ttu-id="4a11e-118">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="4a11e-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a11e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a11e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="4a11e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a11e-120">Request headers</span></span>

| <span data-ttu-id="4a11e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4a11e-121">Name</span></span>       | <span data-ttu-id="4a11e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4a11e-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4a11e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a11e-123">Authorization</span></span>  | <span data-ttu-id="4a11e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a11e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a11e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a11e-126">Request body</span></span>

<span data-ttu-id="4a11e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a11e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a11e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a11e-128">Response</span></span>

<span data-ttu-id="4a11e-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект itemInsightsSettings](../resources/iteminsightssettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a11e-129">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="4a11e-130">**Примечание:** Эта операция проверяет достоверность значений свойств указанного ресурса **itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="4a11e-130">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="4a11e-131">Если свойство **отключеноForGroup,** эта операция не проверяет наличие соответствующей группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a11e-131">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="4a11e-132">Это означает, что если вы установите **disabledForGroup** в группу Azure AD, которая не существовала или была удалена после этого, эта операция не сможет идентифицировать членство в группе и отключить сведения о элементах для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a11e-132">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="4a11e-133">Если **установлено isEnabledInOrganization,** операция позволит получить сведения для всех `true` пользователей организации.</span><span class="sxs-lookup"><span data-stu-id="4a11e-133">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="4a11e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4a11e-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4a11e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a11e-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4a11e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a11e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="4a11e-137">C#</span><span class="sxs-lookup"><span data-stu-id="4a11e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a11e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a11e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a11e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a11e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a11e-140">Java</span><span class="sxs-lookup"><span data-stu-id="4a11e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4a11e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a11e-141">Response</span></span>

<span data-ttu-id="4a11e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a11e-142">Here is an example of the response.</span></span> 
> <span data-ttu-id="4a11e-143">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4a11e-143">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a11e-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a11e-144">All of the properties will be returned from an actual call.</span></span>

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


