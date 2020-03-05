---
title: Обновление политики
description: Обновление свойств в существующей политике.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 81c9d429ba3a74d854a9d091f6e40af7993916f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455494"
---
# <a name="update-policy"></a><span data-ttu-id="19909-103">Обновление политики</span><span class="sxs-lookup"><span data-stu-id="19909-103">Update Policy</span></span>

<span data-ttu-id="19909-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="19909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19909-105">Обновление свойств в существующей [политике](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="19909-105">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="19909-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19909-106">Permissions</span></span>
<span data-ttu-id="19909-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19909-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19909-109">Permission type</span></span>      | <span data-ttu-id="19909-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19909-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19909-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19909-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19909-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19909-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19909-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19909-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19909-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19909-114">Not supported.</span></span>    |
|<span data-ttu-id="19909-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19909-115">Application</span></span> | <span data-ttu-id="19909-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19909-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19909-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19909-117">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="19909-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19909-118">Request headers</span></span>
| <span data-ttu-id="19909-119">Имя</span><span class="sxs-lookup"><span data-stu-id="19909-119">Name</span></span>       | <span data-ttu-id="19909-120">Тип</span><span class="sxs-lookup"><span data-stu-id="19909-120">Type</span></span> | <span data-ttu-id="19909-121">Описание</span><span class="sxs-lookup"><span data-stu-id="19909-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19909-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19909-122">Authorization</span></span>  | <span data-ttu-id="19909-123">string</span><span class="sxs-lookup"><span data-stu-id="19909-123">string</span></span>  | <span data-ttu-id="19909-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19909-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19909-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19909-126">Content-Type</span></span> | <span data-ttu-id="19909-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19909-127">application/json</span></span>  | <span data-ttu-id="19909-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19909-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19909-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19909-130">Request body</span></span>
<span data-ttu-id="19909-131">В тексте запроса укажите объект JSON с параметрами, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="19909-131">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="19909-132">В следующей таблице приведены возможные параметры.</span><span class="sxs-lookup"><span data-stu-id="19909-132">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="19909-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="19909-133">Parameter</span></span>    | <span data-ttu-id="19909-134">Тип</span><span class="sxs-lookup"><span data-stu-id="19909-134">Type</span></span>   |<span data-ttu-id="19909-135">Описание</span><span class="sxs-lookup"><span data-stu-id="19909-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19909-136">RDLC</span><span class="sxs-lookup"><span data-stu-id="19909-136">definition</span></span>|<span data-ttu-id="19909-137">String</span><span class="sxs-lookup"><span data-stu-id="19909-137">String</span></span>|<span data-ttu-id="19909-138">Версия преобразованного объекта [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="19909-138">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="19909-139">displayName</span><span class="sxs-lookup"><span data-stu-id="19909-139">displayName</span></span>|<span data-ttu-id="19909-140">Строка</span><span class="sxs-lookup"><span data-stu-id="19909-140">String</span></span>|<span data-ttu-id="19909-141">Настраиваемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="19909-141">A custom name for the policy.</span></span>|
|<span data-ttu-id="19909-142">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="19909-142">isOrganizationDefault</span></span>|<span data-ttu-id="19909-143">Логический</span><span class="sxs-lookup"><span data-stu-id="19909-143">Boolean</span></span>|<span data-ttu-id="19909-144">Указывает, применяется ли эта политика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19909-144">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="19909-145">type</span><span class="sxs-lookup"><span data-stu-id="19909-145">type</span></span>|<span data-ttu-id="19909-146">String</span><span class="sxs-lookup"><span data-stu-id="19909-146">String</span></span>|<span data-ttu-id="19909-147">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="19909-147">Specifies the type of policy.</span></span> <span data-ttu-id="19909-148">В настоящее время должен быть "Токенлифетимеполици"</span><span class="sxs-lookup"><span data-stu-id="19909-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="19909-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="19909-149">Response</span></span>

<span data-ttu-id="19909-150">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="19909-150">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="19909-151">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="19909-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="19909-152">Пример</span><span class="sxs-lookup"><span data-stu-id="19909-152">Example</span></span>
<span data-ttu-id="19909-153">В следующем примере показано, как обновить определение политики срока действия маркера и задать его в качестве значения по умолчанию для Организации.</span><span class="sxs-lookup"><span data-stu-id="19909-153">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="19909-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="19909-154">Request</span></span>
<span data-ttu-id="19909-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19909-155">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="19909-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="19909-156">Response</span></span>
<span data-ttu-id="19909-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19909-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
