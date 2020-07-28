---
title: Обновление Итеминсигхтс
description: Обновление свойств объекта Итеминсигхтссеттингс
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: de19cf6f33ed0c5b1930077232945564115cd14a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435007"
---
# <a name="update-iteminsightssettings"></a><span data-ttu-id="82d29-103">Обновление Итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="82d29-103">Update itemInsightsSettings</span></span>

<span data-ttu-id="82d29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82d29-105">Обновление свойств указанного ресурса [итеминсигхтссеттингс](../resources/iteminsightssettings.md) .</span><span class="sxs-lookup"><span data-stu-id="82d29-105">Update properties of the specified [itemInsightsSettings](../resources/iteminsightssettings.md) resource.</span></span>

<span data-ttu-id="82d29-106">Сведения о том, как настроить конфиденциальность сведений об элементах для вашей организации, можно узнать в разделе [Настройка конфиденциальности Insights](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="82d29-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="82d29-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82d29-107">Permissions</span></span>

<span data-ttu-id="82d29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82d29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d29-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82d29-110">Permission type</span></span>      | <span data-ttu-id="82d29-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82d29-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82d29-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82d29-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82d29-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82d29-113">User.ReadWrite</span></span> |
|<span data-ttu-id="82d29-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82d29-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82d29-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d29-115">Not supported.</span></span>    |
|<span data-ttu-id="82d29-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82d29-116">Application</span></span> | <span data-ttu-id="82d29-117">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82d29-117">User.ReadWrite</span></span> |

><span data-ttu-id="82d29-118">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="82d29-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="82d29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82d29-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="82d29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82d29-120">Request headers</span></span>

| <span data-ttu-id="82d29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82d29-121">Header</span></span>       | <span data-ttu-id="82d29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82d29-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="82d29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82d29-123">Authorization</span></span>  | <span data-ttu-id="82d29-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82d29-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82d29-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82d29-126">Content-Type</span></span>  | <span data-ttu-id="82d29-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82d29-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82d29-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82d29-128">Request body</span></span>

<span data-ttu-id="82d29-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="82d29-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="82d29-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="82d29-132">Property</span></span>     | <span data-ttu-id="82d29-133">Тип</span><span class="sxs-lookup"><span data-stu-id="82d29-133">Type</span></span>   |<span data-ttu-id="82d29-134">Описание</span><span class="sxs-lookup"><span data-stu-id="82d29-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82d29-135">исенаблединорганизатион</span><span class="sxs-lookup"><span data-stu-id="82d29-135">isEnabledInOrganization</span></span>|<span data-ttu-id="82d29-136">Логический</span><span class="sxs-lookup"><span data-stu-id="82d29-136">Boolean</span></span>| <span data-ttu-id="82d29-137">`true`, если аналитика элемента организации включена; `false`Если аналитика элемента Организации отключена для всех пользователей без исключений.</span><span class="sxs-lookup"><span data-stu-id="82d29-137">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="82d29-138">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="82d29-138">Default is `true`.</span></span> <span data-ttu-id="82d29-139">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="82d29-139">Optional.</span></span>|
|<span data-ttu-id="82d29-140">дисабледфорграуп</span><span class="sxs-lookup"><span data-stu-id="82d29-140">disabledForGroup</span></span>|<span data-ttu-id="82d29-141">Строка</span><span class="sxs-lookup"><span data-stu-id="82d29-141">String</span></span>| <span data-ttu-id="82d29-142">Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники".</span><span class="sxs-lookup"><span data-stu-id="82d29-142">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="82d29-143">Значение по умолчанию: `empty`.</span><span class="sxs-lookup"><span data-stu-id="82d29-143">Default is `empty`.</span></span> <span data-ttu-id="82d29-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="82d29-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="82d29-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d29-145">Response</span></span>

<span data-ttu-id="82d29-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итеминсигхтссеттингс](../resources/iteminsightssettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82d29-146">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="82d29-147">**Примечание:** Эта операция проверяет допустимость значений свойств указанного ресурса **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="82d29-147">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="82d29-148">Если задано свойство **дисабледфорграуп** , эта операция не проверяет существование соответствующей группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82d29-148">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="82d29-149">Это означает, что если вы настроили **дисабледфорграуп** для группы Azure AD, которая не существовала или была удалена, то эта операция не сможет определить членство в группах и отключить сведения об элементе для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="82d29-149">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="82d29-150">Если для параметра **исенаблединорганизатион** задано значение `true` , операция позволит получить информацию для всех пользователей в Организации.</span><span class="sxs-lookup"><span data-stu-id="82d29-150">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="82d29-151">Пример</span><span class="sxs-lookup"><span data-stu-id="82d29-151">Example</span></span> 

### <a name="request"></a><span data-ttu-id="82d29-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="82d29-152">Request</span></span>

<span data-ttu-id="82d29-153">Ниже приведен пример запроса на изменение параметров конфиденциальности "**дисабледфорграуп**" для администраторов, чтобы запретить отображение элемента для определенной группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82d29-153">Here is an example request on how admin updates "**disabledForGroup**" privacy setting in order to prohibit displaying users' item insights of a particular Azure AD group.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```

##### <a name="response"></a><span data-ttu-id="82d29-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d29-154">Response</span></span>

<span data-ttu-id="82d29-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82d29-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
