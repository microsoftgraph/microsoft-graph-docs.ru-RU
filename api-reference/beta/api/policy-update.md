---
title: Обновление политики
description: Обновление свойств в существующей политике.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 1194d746d0313da0835fc9939bc12671c372684d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408256"
---
# <a name="update-policy"></a><span data-ttu-id="a6a33-103">Обновление политики</span><span class="sxs-lookup"><span data-stu-id="a6a33-103">Update Policy</span></span>

<span data-ttu-id="a6a33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6a33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6a33-105">Обновление свойств в существующей [политике](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="a6a33-105">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6a33-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6a33-106">Permissions</span></span>
<span data-ttu-id="a6a33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6a33-109">Permission type</span></span>      | <span data-ttu-id="a6a33-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6a33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6a33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6a33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6a33-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6a33-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6a33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6a33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6a33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a33-114">Not supported.</span></span>    |
|<span data-ttu-id="a6a33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6a33-115">Application</span></span> | <span data-ttu-id="a6a33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a33-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6a33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6a33-117">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a6a33-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6a33-118">Request headers</span></span>
| <span data-ttu-id="a6a33-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a6a33-119">Name</span></span>       | <span data-ttu-id="a6a33-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a6a33-120">Type</span></span> | <span data-ttu-id="a6a33-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a6a33-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6a33-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6a33-122">Authorization</span></span>  | <span data-ttu-id="a6a33-123">string</span><span class="sxs-lookup"><span data-stu-id="a6a33-123">string</span></span>  | <span data-ttu-id="a6a33-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6a33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6a33-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6a33-126">Content-Type</span></span> | <span data-ttu-id="a6a33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a6a33-127">application/json</span></span>  | <span data-ttu-id="a6a33-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6a33-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6a33-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6a33-130">Request body</span></span>
<span data-ttu-id="a6a33-131">В тексте запроса укажите объект JSON с параметрами, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a6a33-131">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="a6a33-132">В следующей таблице приведены возможные параметры.</span><span class="sxs-lookup"><span data-stu-id="a6a33-132">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="a6a33-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="a6a33-133">Parameter</span></span>    | <span data-ttu-id="a6a33-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a6a33-134">Type</span></span>   |<span data-ttu-id="a6a33-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a6a33-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6a33-136">RDLC</span><span class="sxs-lookup"><span data-stu-id="a6a33-136">definition</span></span>|<span data-ttu-id="a6a33-137">String</span><span class="sxs-lookup"><span data-stu-id="a6a33-137">String</span></span>|<span data-ttu-id="a6a33-138">Версия преобразованного объекта [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="a6a33-138">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="a6a33-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a33-139">displayName</span></span>|<span data-ttu-id="a6a33-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a6a33-140">String</span></span>|<span data-ttu-id="a6a33-141">Настраиваемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="a6a33-141">A custom name for the policy.</span></span>|
|<span data-ttu-id="a6a33-142">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="a6a33-142">isOrganizationDefault</span></span>|<span data-ttu-id="a6a33-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6a33-143">Boolean</span></span>|<span data-ttu-id="a6a33-144">Указывает, применяется ли эта политика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a33-144">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="a6a33-145">type</span><span class="sxs-lookup"><span data-stu-id="a6a33-145">type</span></span>|<span data-ttu-id="a6a33-146">String</span><span class="sxs-lookup"><span data-stu-id="a6a33-146">String</span></span>|<span data-ttu-id="a6a33-147">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="a6a33-147">Specifies the type of policy.</span></span> <span data-ttu-id="a6a33-148">В настоящее время должен быть "Токенлифетимеполици"</span><span class="sxs-lookup"><span data-stu-id="a6a33-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="a6a33-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6a33-149">Response</span></span>

<span data-ttu-id="a6a33-150">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a6a33-150">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="a6a33-151">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="a6a33-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="a6a33-152">Пример</span><span class="sxs-lookup"><span data-stu-id="a6a33-152">Example</span></span>
<span data-ttu-id="a6a33-153">В следующем примере показано, как обновить определение политики срока действия маркера и задать его в качестве значения по умолчанию для Организации.</span><span class="sxs-lookup"><span data-stu-id="a6a33-153">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="a6a33-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6a33-154">Request</span></span>
<span data-ttu-id="a6a33-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6a33-155">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="a6a33-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6a33-156">Response</span></span>
<span data-ttu-id="a6a33-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6a33-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
