---
title: Создание networkIPv6ConfigurationManagementCondition
description: Создание нового объекта networkIPv6ConfigurationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 230c55ae7cce8231c660eed73da01d82a3eae5f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881853"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="44701-103">Создание networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="44701-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="44701-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44701-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44701-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44701-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44701-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="44701-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44701-107">Создание нового объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="44701-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44701-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44701-108">Prerequisites</span></span>
<span data-ttu-id="44701-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44701-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44701-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44701-111">Permission type</span></span>|<span data-ttu-id="44701-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44701-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44701-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44701-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44701-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44701-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44701-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44701-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44701-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44701-116">Not supported.</span></span>|
|<span data-ttu-id="44701-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44701-117">Application</span></span>|<span data-ttu-id="44701-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44701-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44701-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44701-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="44701-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44701-120">Request headers</span></span>
|<span data-ttu-id="44701-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44701-121">Header</span></span>|<span data-ttu-id="44701-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44701-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44701-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44701-123">Authorization</span></span>|<span data-ttu-id="44701-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="44701-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44701-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44701-125">Accept</span></span>|<span data-ttu-id="44701-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44701-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44701-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44701-127">Request body</span></span>
<span data-ttu-id="44701-128">В тексте запроса укажите представление JSON для объекта networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="44701-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="44701-129">В следующей таблице показаны свойства, которые необходимы для создания networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="44701-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="44701-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44701-130">Property</span></span>|<span data-ttu-id="44701-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44701-131">Type</span></span>|<span data-ttu-id="44701-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44701-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44701-133">id</span><span class="sxs-lookup"><span data-stu-id="44701-133">id</span></span>|<span data-ttu-id="44701-134">Строка</span><span class="sxs-lookup"><span data-stu-id="44701-134">String</span></span>|<span data-ttu-id="44701-135">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="44701-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="44701-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="44701-136">System generated value assigned when created.</span></span> <span data-ttu-id="44701-137">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-138">уникального имени</span><span class="sxs-lookup"><span data-stu-id="44701-138">uniqueName</span></span>|<span data-ttu-id="44701-139">Строка</span><span class="sxs-lookup"><span data-stu-id="44701-139">String</span></span>|<span data-ttu-id="44701-140">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="44701-140">Unique name for the management condition.</span></span> <span data-ttu-id="44701-141">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="44701-141">Used in management condition expressions.</span></span> <span data-ttu-id="44701-142">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-143">displayName</span><span class="sxs-lookup"><span data-stu-id="44701-143">displayName</span></span>|<span data-ttu-id="44701-144">Строка</span><span class="sxs-lookup"><span data-stu-id="44701-144">String</span></span>|<span data-ttu-id="44701-145">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="44701-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="44701-146">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-147">описание</span><span class="sxs-lookup"><span data-stu-id="44701-147">description</span></span>|<span data-ttu-id="44701-148">Строка</span><span class="sxs-lookup"><span data-stu-id="44701-148">String</span></span>|<span data-ttu-id="44701-149">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="44701-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="44701-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44701-151">createdDateTime</span></span>|<span data-ttu-id="44701-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44701-152">DateTimeOffset</span></span>|<span data-ttu-id="44701-153">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="44701-153">The time the management condition was created.</span></span> <span data-ttu-id="44701-154">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="44701-154">Generated service side.</span></span> <span data-ttu-id="44701-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44701-156">modifiedDateTime</span></span>|<span data-ttu-id="44701-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44701-157">DateTimeOffset</span></span>|<span data-ttu-id="44701-158">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="44701-158">The time the management condition was last modified.</span></span> <span data-ttu-id="44701-159">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="44701-159">Updated service side.</span></span> <span data-ttu-id="44701-160">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-161">eTag</span><span class="sxs-lookup"><span data-stu-id="44701-161">eTag</span></span>|<span data-ttu-id="44701-162">String</span><span class="sxs-lookup"><span data-stu-id="44701-162">String</span></span>|<span data-ttu-id="44701-163">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="44701-163">ETag of the management condition.</span></span> <span data-ttu-id="44701-164">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="44701-164">Updated service side.</span></span> <span data-ttu-id="44701-165">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="44701-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="44701-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="44701-166">applicablePlatforms</span></span>|<span data-ttu-id="44701-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="44701-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="44701-168">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="44701-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="44701-169">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="44701-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="44701-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="44701-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="44701-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="44701-171">ipV6Prefix</span></span>|<span data-ttu-id="44701-172">Строка</span><span class="sxs-lookup"><span data-stu-id="44701-172">String</span></span>|<span data-ttu-id="44701-173">Подсеть IP версии 6, подключенных к.</span><span class="sxs-lookup"><span data-stu-id="44701-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="44701-174">например 2001:db8:: / 32</span><span class="sxs-lookup"><span data-stu-id="44701-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="44701-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="44701-175">ipV6Gateway</span></span>|<span data-ttu-id="44701-176">Строка</span><span class="sxs-lookup"><span data-stu-id="44701-176">String</span></span>|<span data-ttu-id="44701-177">Адрес шлюза IP версии 6 для.</span><span class="sxs-lookup"><span data-stu-id="44701-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="44701-178">например 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="44701-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="44701-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="44701-179">ipV6DNSServerList</span></span>|<span data-ttu-id="44701-180">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44701-180">String collection</span></span>|<span data-ttu-id="44701-181">Серверы IPv6 DNS, настроенные для адаптера.</span><span class="sxs-lookup"><span data-stu-id="44701-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="44701-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="44701-182">dnsSuffixList</span></span>|<span data-ttu-id="44701-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44701-183">String collection</span></span>|<span data-ttu-id="44701-184">Допустимое DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="44701-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="44701-185">Например seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="44701-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="44701-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="44701-186">Response</span></span>
<span data-ttu-id="44701-187">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44701-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44701-188">Пример</span><span class="sxs-lookup"><span data-stu-id="44701-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="44701-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="44701-189">Request</span></span>
<span data-ttu-id="44701-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44701-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="44701-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="44701-191">Response</span></span>
<span data-ttu-id="44701-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="44701-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





