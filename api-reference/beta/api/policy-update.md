---
title: Обновление политики
description: Обновление свойств в существующей политике.
localization_priority: Normal
ms.openlocfilehash: 53b7af8966c932598328e8b78e76022ca6db9c8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337405"
---
# <a name="update-policy"></a><span data-ttu-id="0efbb-103">Обновление политики</span><span class="sxs-lookup"><span data-stu-id="0efbb-103">Update Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0efbb-104">Обновление свойств в существующей [политике](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="0efbb-104">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0efbb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0efbb-105">Permissions</span></span>
<span data-ttu-id="0efbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0efbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0efbb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0efbb-108">Permission type</span></span>      | <span data-ttu-id="0efbb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0efbb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0efbb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0efbb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0efbb-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0efbb-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0efbb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0efbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0efbb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0efbb-113">Not supported.</span></span>    |
|<span data-ttu-id="0efbb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0efbb-114">Application</span></span> | <span data-ttu-id="0efbb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0efbb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0efbb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0efbb-116">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0efbb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0efbb-117">Request headers</span></span>
| <span data-ttu-id="0efbb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0efbb-118">Name</span></span>       | <span data-ttu-id="0efbb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0efbb-119">Type</span></span> | <span data-ttu-id="0efbb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0efbb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0efbb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0efbb-121">Authorization</span></span>  | <span data-ttu-id="0efbb-122">string</span><span class="sxs-lookup"><span data-stu-id="0efbb-122">string</span></span>  | <span data-ttu-id="0efbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0efbb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0efbb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0efbb-125">Content-Type</span></span> | <span data-ttu-id="0efbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0efbb-126">application/json</span></span>  | <span data-ttu-id="0efbb-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0efbb-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0efbb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0efbb-129">Request body</span></span>
<span data-ttu-id="0efbb-130">В тексте запроса укажите объект JSON с параметрами, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0efbb-130">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="0efbb-131">В следующей таблице приведены возможные параметры.</span><span class="sxs-lookup"><span data-stu-id="0efbb-131">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="0efbb-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="0efbb-132">Parameter</span></span>    | <span data-ttu-id="0efbb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0efbb-133">Type</span></span>   |<span data-ttu-id="0efbb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0efbb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0efbb-135">RDLC</span><span class="sxs-lookup"><span data-stu-id="0efbb-135">definition</span></span>|<span data-ttu-id="0efbb-136">String</span><span class="sxs-lookup"><span data-stu-id="0efbb-136">String</span></span>|<span data-ttu-id="0efbb-137">Версия преобразованного объекта [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="0efbb-137">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="0efbb-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0efbb-138">displayName</span></span>|<span data-ttu-id="0efbb-139">String</span><span class="sxs-lookup"><span data-stu-id="0efbb-139">String</span></span>|<span data-ttu-id="0efbb-140">Настраиваемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0efbb-140">A custom name for the policy.</span></span>|
|<span data-ttu-id="0efbb-141">Исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="0efbb-141">isOrganizationDefault</span></span>|<span data-ttu-id="0efbb-142">Логический</span><span class="sxs-lookup"><span data-stu-id="0efbb-142">Boolean</span></span>|<span data-ttu-id="0efbb-143">Указывает, применяется ли эта политика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0efbb-143">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="0efbb-144">type</span><span class="sxs-lookup"><span data-stu-id="0efbb-144">type</span></span>|<span data-ttu-id="0efbb-145">String</span><span class="sxs-lookup"><span data-stu-id="0efbb-145">String</span></span>|<span data-ttu-id="0efbb-146">Указывает тип политики.</span><span class="sxs-lookup"><span data-stu-id="0efbb-146">Specifies the type of policy.</span></span> <span data-ttu-id="0efbb-147">В настоящее время должен быть "Токенлифетимеполици"</span><span class="sxs-lookup"><span data-stu-id="0efbb-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="0efbb-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="0efbb-148">Response</span></span>

<span data-ttu-id="0efbb-149">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0efbb-149">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="0efbb-150">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="0efbb-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="0efbb-151">Пример</span><span class="sxs-lookup"><span data-stu-id="0efbb-151">Example</span></span>
<span data-ttu-id="0efbb-152">В следующем примере показано, как обновить определение политики срока действия маркера и задать его в качестве значения по умолчанию для Организации.</span><span class="sxs-lookup"><span data-stu-id="0efbb-152">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="0efbb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0efbb-153">Request</span></span>
<span data-ttu-id="0efbb-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0efbb-154">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="0efbb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0efbb-155">Response</span></span>
<span data-ttu-id="0efbb-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0efbb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
