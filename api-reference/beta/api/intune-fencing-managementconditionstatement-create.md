---
title: Создание managementConditionStatement
description: Создание нового объекта managementConditionStatement.
author: tfitzmac
ms.openlocfilehash: 5402faee0c7ace84957f3ff6a2ef65844f5a527e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327351"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="1ceec-103">Создание managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="1ceec-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="1ceec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1ceec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ceec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ceec-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ceec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ceec-107">Создание нового объекта [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="1ceec-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ceec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ceec-108">Prerequisites</span></span>
<span data-ttu-id="1ceec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ceec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ceec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ceec-111">Permission type</span></span>|<span data-ttu-id="1ceec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ceec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ceec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ceec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ceec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ceec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ceec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ceec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ceec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceec-116">Not supported.</span></span>|
|<span data-ttu-id="1ceec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ceec-117">Application</span></span>|<span data-ttu-id="1ceec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ceec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ceec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="1ceec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ceec-120">Request headers</span></span>
|<span data-ttu-id="1ceec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ceec-121">Header</span></span>|<span data-ttu-id="1ceec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ceec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ceec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ceec-123">Authorization</span></span>|<span data-ttu-id="1ceec-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1ceec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ceec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ceec-125">Accept</span></span>|<span data-ttu-id="1ceec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ceec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ceec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ceec-127">Request body</span></span>
<span data-ttu-id="1ceec-128">В тексте запроса укажите представление JSON для объекта managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="1ceec-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="1ceec-129">В следующей таблице показаны свойства, которые необходимы для создания managementConditionStatement.</span><span class="sxs-lookup"><span data-stu-id="1ceec-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="1ceec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ceec-130">Property</span></span>|<span data-ttu-id="1ceec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ceec-131">Type</span></span>|<span data-ttu-id="1ceec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ceec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ceec-133">id</span><span class="sxs-lookup"><span data-stu-id="1ceec-133">id</span></span>|<span data-ttu-id="1ceec-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1ceec-134">String</span></span>|<span data-ttu-id="1ceec-135">Уникальный идентификатор для управления условная инструкция.</span><span class="sxs-lookup"><span data-stu-id="1ceec-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="1ceec-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="1ceec-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1ceec-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ceec-137">displayName</span></span>|<span data-ttu-id="1ceec-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1ceec-138">String</span></span>|<span data-ttu-id="1ceec-139">Имя оператора условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="1ceec-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="1ceec-140">описание</span><span class="sxs-lookup"><span data-stu-id="1ceec-140">description</span></span>|<span data-ttu-id="1ceec-141">Строка</span><span class="sxs-lookup"><span data-stu-id="1ceec-141">String</span></span>|<span data-ttu-id="1ceec-142">Описание управления условная инструкция определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="1ceec-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="1ceec-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ceec-143">createdDateTime</span></span>|<span data-ttu-id="1ceec-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ceec-144">DateTimeOffset</span></span>|<span data-ttu-id="1ceec-145">Время создания условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="1ceec-145">The time the management condition statement was created.</span></span> <span data-ttu-id="1ceec-146">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="1ceec-146">Generated service side.</span></span>|
|<span data-ttu-id="1ceec-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ceec-147">modifiedDateTime</span></span>|<span data-ttu-id="1ceec-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ceec-148">DateTimeOffset</span></span>|<span data-ttu-id="1ceec-149">Время последнего изменения условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="1ceec-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="1ceec-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="1ceec-150">Updated service side.</span></span>|
|<span data-ttu-id="1ceec-151">выражение</span><span class="sxs-lookup"><span data-stu-id="1ceec-151">expression</span></span>|[<span data-ttu-id="1ceec-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="1ceec-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="1ceec-153">Выражение оператора условия управления, используется для оценки Если инструкции с условием управления был активирован деактивирован.</span><span class="sxs-lookup"><span data-stu-id="1ceec-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="1ceec-154">eTag</span><span class="sxs-lookup"><span data-stu-id="1ceec-154">eTag</span></span>|<span data-ttu-id="1ceec-155">String</span><span class="sxs-lookup"><span data-stu-id="1ceec-155">String</span></span>|<span data-ttu-id="1ceec-156">ETag условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="1ceec-156">ETag of the management condition statement.</span></span> <span data-ttu-id="1ceec-157">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="1ceec-157">Updated service side.</span></span>|
|<span data-ttu-id="1ceec-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1ceec-158">applicablePlatforms</span></span>|<span data-ttu-id="1ceec-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1ceec-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1ceec-160">Применимые платформы для этой условная инструкция управления.</span><span class="sxs-lookup"><span data-stu-id="1ceec-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="1ceec-161">Отсчитывается от нужна условия управления, связанные с управлением условие оператора и поиск пересечения применимых платформ.</span><span class="sxs-lookup"><span data-stu-id="1ceec-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="1ceec-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="1ceec-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ceec-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ceec-163">Response</span></span>
<span data-ttu-id="1ceec-164">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1ceec-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ceec-165">Пример</span><span class="sxs-lookup"><span data-stu-id="1ceec-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ceec-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ceec-166">Request</span></span>
<span data-ttu-id="1ceec-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ceec-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1ceec-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ceec-168">Response</span></span>
<span data-ttu-id="1ceec-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1ceec-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```





