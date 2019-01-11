---
title: Обновление политики
description: Обновление свойств в уже существующей политики.
localization_priority: Normal
ms.openlocfilehash: 2992f2f76c0e8b213ad8aabca1bfd0fe59883989
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857157"
---
# <a name="update-policy"></a><span data-ttu-id="05109-103">Обновление политики</span><span class="sxs-lookup"><span data-stu-id="05109-103">Update Policy</span></span>

> <span data-ttu-id="05109-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05109-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05109-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05109-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05109-106">Обновление свойств в уже существующей [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="05109-106">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05109-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05109-107">Permissions</span></span>
<span data-ttu-id="05109-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05109-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05109-110">Permission type</span></span>      | <span data-ttu-id="05109-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05109-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05109-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05109-112">Delegated (work or school account)</span></span> | <span data-ttu-id="05109-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05109-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05109-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05109-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05109-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05109-115">Not supported.</span></span>    |
|<span data-ttu-id="05109-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05109-116">Application</span></span> | <span data-ttu-id="05109-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05109-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05109-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05109-118">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="05109-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05109-119">Request headers</span></span>
| <span data-ttu-id="05109-120">Имя</span><span class="sxs-lookup"><span data-stu-id="05109-120">Name</span></span>       | <span data-ttu-id="05109-121">Тип</span><span class="sxs-lookup"><span data-stu-id="05109-121">Type</span></span> | <span data-ttu-id="05109-122">Описание</span><span class="sxs-lookup"><span data-stu-id="05109-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05109-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05109-123">Authorization</span></span>  | <span data-ttu-id="05109-124">string</span><span class="sxs-lookup"><span data-stu-id="05109-124">string</span></span>  | <span data-ttu-id="05109-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05109-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05109-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05109-127">Content-Type</span></span> | <span data-ttu-id="05109-128">application/json</span><span class="sxs-lookup"><span data-stu-id="05109-128">application/json</span></span>  | <span data-ttu-id="05109-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05109-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05109-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05109-131">Request body</span></span>
<span data-ttu-id="05109-132">В тексте запроса укажите объект JSON вместе с параметрами, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="05109-132">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="05109-133">В следующей таблице показаны возможные параметры.</span><span class="sxs-lookup"><span data-stu-id="05109-133">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="05109-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="05109-134">Parameter</span></span>    | <span data-ttu-id="05109-135">Тип</span><span class="sxs-lookup"><span data-stu-id="05109-135">Type</span></span>   |<span data-ttu-id="05109-136">Описание</span><span class="sxs-lookup"><span data-stu-id="05109-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05109-137">definition</span><span class="sxs-lookup"><span data-stu-id="05109-137">definition</span></span>|<span data-ttu-id="05109-138">Строка</span><span class="sxs-lookup"><span data-stu-id="05109-138">String</span></span>|<span data-ttu-id="05109-139">Stringified версия объекта [политики](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="05109-139">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="05109-140">displayName</span><span class="sxs-lookup"><span data-stu-id="05109-140">displayName</span></span>|<span data-ttu-id="05109-141">Строка</span><span class="sxs-lookup"><span data-stu-id="05109-141">String</span></span>|<span data-ttu-id="05109-142">Пользовательское имя для политики.</span><span class="sxs-lookup"><span data-stu-id="05109-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="05109-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="05109-143">isOrganizationDefault</span></span>|<span data-ttu-id="05109-144">Логический</span><span class="sxs-lookup"><span data-stu-id="05109-144">Boolean</span></span>|<span data-ttu-id="05109-145">Указывает, если эта политика будет применяться по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="05109-145">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="05109-146">type</span><span class="sxs-lookup"><span data-stu-id="05109-146">type</span></span>|<span data-ttu-id="05109-147">Строка</span><span class="sxs-lookup"><span data-stu-id="05109-147">String</span></span>|<span data-ttu-id="05109-148">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="05109-148">Specifies the type of policy.</span></span> <span data-ttu-id="05109-149">В настоящее время должен быть «TokenLifetimePolicy»</span><span class="sxs-lookup"><span data-stu-id="05109-149">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="05109-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="05109-150">Response</span></span>

<span data-ttu-id="05109-151">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="05109-151">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="05109-152">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="05109-152">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="05109-153">Пример</span><span class="sxs-lookup"><span data-stu-id="05109-153">Example</span></span>
<span data-ttu-id="05109-154">В следующем примере происходит обновление определения срока действия маркера и устанавливает ее в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="05109-154">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="05109-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="05109-155">Request</span></span>
<span data-ttu-id="05109-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05109-156">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="05109-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="05109-157">Response</span></span>
<span data-ttu-id="05109-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05109-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
