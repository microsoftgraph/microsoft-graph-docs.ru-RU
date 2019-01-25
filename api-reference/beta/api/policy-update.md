---
title: Обновление политики
description: Обновление свойств в уже существующей политики.
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515414"
---
# <a name="update-policy"></a><span data-ttu-id="0d2a0-103">Обновление политики</span><span class="sxs-lookup"><span data-stu-id="0d2a0-103">Update Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d2a0-104">Обновление свойств в уже существующей [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="0d2a0-104">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d2a0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2a0-105">Permissions</span></span>
<span data-ttu-id="0d2a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d2a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2a0-108">Permission type</span></span>      | <span data-ttu-id="0d2a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d2a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d2a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d2a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d2a0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d2a0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d2a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d2a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d2a0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-113">Not supported.</span></span>    |
|<span data-ttu-id="0d2a0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d2a0-114">Application</span></span> | <span data-ttu-id="0d2a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d2a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d2a0-116">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0d2a0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d2a0-117">Request headers</span></span>
| <span data-ttu-id="0d2a0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0d2a0-118">Name</span></span>       | <span data-ttu-id="0d2a0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0d2a0-119">Type</span></span> | <span data-ttu-id="0d2a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0d2a0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d2a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d2a0-121">Authorization</span></span>  | <span data-ttu-id="0d2a0-122">string</span><span class="sxs-lookup"><span data-stu-id="0d2a0-122">string</span></span>  | <span data-ttu-id="0d2a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d2a0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d2a0-125">Content-Type</span></span> | <span data-ttu-id="0d2a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d2a0-126">application/json</span></span>  | <span data-ttu-id="0d2a0-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d2a0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d2a0-129">Request body</span></span>
<span data-ttu-id="0d2a0-130">В тексте запроса укажите объект JSON вместе с параметрами, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-130">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="0d2a0-131">В следующей таблице показаны возможные параметры.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-131">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="0d2a0-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d2a0-132">Parameter</span></span>    | <span data-ttu-id="0d2a0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0d2a0-133">Type</span></span>   |<span data-ttu-id="0d2a0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0d2a0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d2a0-135">definition</span><span class="sxs-lookup"><span data-stu-id="0d2a0-135">definition</span></span>|<span data-ttu-id="0d2a0-136">String</span><span class="sxs-lookup"><span data-stu-id="0d2a0-136">String</span></span>|<span data-ttu-id="0d2a0-137">Stringified версия объекта [политики](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="0d2a0-137">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="0d2a0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0d2a0-138">displayName</span></span>|<span data-ttu-id="0d2a0-139">String</span><span class="sxs-lookup"><span data-stu-id="0d2a0-139">String</span></span>|<span data-ttu-id="0d2a0-140">Пользовательское имя для политики.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-140">A custom name for the policy.</span></span>|
|<span data-ttu-id="0d2a0-141">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="0d2a0-141">isOrganizationDefault</span></span>|<span data-ttu-id="0d2a0-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="0d2a0-142">Boolean</span></span>|<span data-ttu-id="0d2a0-143">Указывает, если эта политика будет применяться по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-143">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="0d2a0-144">type</span><span class="sxs-lookup"><span data-stu-id="0d2a0-144">type</span></span>|<span data-ttu-id="0d2a0-145">String</span><span class="sxs-lookup"><span data-stu-id="0d2a0-145">String</span></span>|<span data-ttu-id="0d2a0-146">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-146">Specifies the type of policy.</span></span> <span data-ttu-id="0d2a0-147">В настоящее время должен быть «TokenLifetimePolicy»</span><span class="sxs-lookup"><span data-stu-id="0d2a0-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="0d2a0-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d2a0-148">Response</span></span>

<span data-ttu-id="0d2a0-149">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-149">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="0d2a0-150">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="0d2a0-151">Пример</span><span class="sxs-lookup"><span data-stu-id="0d2a0-151">Example</span></span>
<span data-ttu-id="0d2a0-152">В следующем примере происходит обновление определения срока действия маркера и устанавливает ее в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-152">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="0d2a0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d2a0-153">Request</span></span>
<span data-ttu-id="0d2a0-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d2a0-154">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="0d2a0-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d2a0-155">Response</span></span>
<span data-ttu-id="0d2a0-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0d2a0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
