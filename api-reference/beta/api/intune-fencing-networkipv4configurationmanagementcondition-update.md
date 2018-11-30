---
title: Обновление networkIPv4ConfigurationManagementCondition
description: Обновление свойства объекта networkIPv4ConfigurationManagementCondition.
ms.openlocfilehash: 21f378b3ce7926e1e0b89f6f448cfcadebce9c69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081770"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="cf998-103">Обновление networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cf998-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="cf998-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf998-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf998-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf998-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf998-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cf998-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf998-107">Обновление свойства объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cf998-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf998-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf998-108">Prerequisites</span></span>
<span data-ttu-id="cf998-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf998-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf998-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf998-111">Permission type</span></span>|<span data-ttu-id="cf998-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf998-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf998-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf998-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf998-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf998-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf998-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf998-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf998-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf998-116">Not supported.</span></span>|
|<span data-ttu-id="cf998-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf998-117">Application</span></span>|<span data-ttu-id="cf998-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf998-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf998-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf998-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="cf998-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf998-120">Request headers</span></span>
|<span data-ttu-id="cf998-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf998-121">Header</span></span>|<span data-ttu-id="cf998-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf998-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf998-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf998-123">Authorization</span></span>|<span data-ttu-id="cf998-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cf998-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf998-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf998-125">Accept</span></span>|<span data-ttu-id="cf998-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf998-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf998-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf998-127">Request body</span></span>
<span data-ttu-id="cf998-128">В тексте запроса укажите представление JSON для объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cf998-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="cf998-129">В следующей таблице показаны свойства, которые необходимы для создания [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="cf998-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="cf998-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf998-130">Property</span></span>|<span data-ttu-id="cf998-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf998-131">Type</span></span>|<span data-ttu-id="cf998-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf998-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf998-133">id</span><span class="sxs-lookup"><span data-stu-id="cf998-133">id</span></span>|<span data-ttu-id="cf998-134">String</span><span class="sxs-lookup"><span data-stu-id="cf998-134">String</span></span>|<span data-ttu-id="cf998-135">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="cf998-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="cf998-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="cf998-136">System generated value assigned when created.</span></span> <span data-ttu-id="cf998-137">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-138">уникального имени</span><span class="sxs-lookup"><span data-stu-id="cf998-138">uniqueName</span></span>|<span data-ttu-id="cf998-139">String</span><span class="sxs-lookup"><span data-stu-id="cf998-139">String</span></span>|<span data-ttu-id="cf998-140">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="cf998-140">Unique name for the management condition.</span></span> <span data-ttu-id="cf998-141">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="cf998-141">Used in management condition expressions.</span></span> <span data-ttu-id="cf998-142">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cf998-143">displayName</span></span>|<span data-ttu-id="cf998-144">String</span><span class="sxs-lookup"><span data-stu-id="cf998-144">String</span></span>|<span data-ttu-id="cf998-145">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="cf998-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="cf998-146">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-147">описание</span><span class="sxs-lookup"><span data-stu-id="cf998-147">description</span></span>|<span data-ttu-id="cf998-148">String</span><span class="sxs-lookup"><span data-stu-id="cf998-148">String</span></span>|<span data-ttu-id="cf998-149">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="cf998-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="cf998-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf998-151">createdDateTime</span></span>|<span data-ttu-id="cf998-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf998-152">DateTimeOffset</span></span>|<span data-ttu-id="cf998-153">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="cf998-153">The time the management condition was created.</span></span> <span data-ttu-id="cf998-154">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="cf998-154">Generated service side.</span></span> <span data-ttu-id="cf998-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf998-156">modifiedDateTime</span></span>|<span data-ttu-id="cf998-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf998-157">DateTimeOffset</span></span>|<span data-ttu-id="cf998-158">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="cf998-158">The time the management condition was last modified.</span></span> <span data-ttu-id="cf998-159">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="cf998-159">Updated service side.</span></span> <span data-ttu-id="cf998-160">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-161">eTag</span><span class="sxs-lookup"><span data-stu-id="cf998-161">eTag</span></span>|<span data-ttu-id="cf998-162">String</span><span class="sxs-lookup"><span data-stu-id="cf998-162">String</span></span>|<span data-ttu-id="cf998-163">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="cf998-163">ETag of the management condition.</span></span> <span data-ttu-id="cf998-164">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="cf998-164">Updated service side.</span></span> <span data-ttu-id="cf998-165">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cf998-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cf998-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cf998-166">applicablePlatforms</span></span>|<span data-ttu-id="cf998-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cf998-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cf998-168">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="cf998-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="cf998-169">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="cf998-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="cf998-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="cf998-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="cf998-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="cf998-171">ipV4Prefix</span></span>|<span data-ttu-id="cf998-172">String</span><span class="sxs-lookup"><span data-stu-id="cf998-172">String</span></span>|<span data-ttu-id="cf998-173">Подсеть IPv4, подключенных к.</span><span class="sxs-lookup"><span data-stu-id="cf998-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="cf998-174">например 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="cf998-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="cf998-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="cf998-175">ipV4Gateway</span></span>|<span data-ttu-id="cf998-176">String</span><span class="sxs-lookup"><span data-stu-id="cf998-176">String</span></span>|<span data-ttu-id="cf998-177">IPv4-адрес шлюза.</span><span class="sxs-lookup"><span data-stu-id="cf998-177">The IPv4 gateway address.</span></span> <span data-ttu-id="cf998-178">например 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="cf998-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="cf998-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="cf998-179">ipV4DHCPServer</span></span>|<span data-ttu-id="cf998-180">String</span><span class="sxs-lookup"><span data-stu-id="cf998-180">String</span></span>|<span data-ttu-id="cf998-181">IPv4-адрес на DHCP-сервер для адаптера.</span><span class="sxs-lookup"><span data-stu-id="cf998-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="cf998-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="cf998-182">ipV4DNSServerList</span></span>|<span data-ttu-id="cf998-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf998-183">String collection</span></span>|<span data-ttu-id="cf998-184">IPv4 DNS-серверов, настроенных для адаптера.</span><span class="sxs-lookup"><span data-stu-id="cf998-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="cf998-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="cf998-185">dnsSuffixList</span></span>|<span data-ttu-id="cf998-186">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf998-186">String collection</span></span>|<span data-ttu-id="cf998-187">Допустимое DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="cf998-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="cf998-188">Например seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="cf998-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="cf998-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf998-189">Response</span></span>
<span data-ttu-id="cf998-190">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cf998-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf998-191">Пример</span><span class="sxs-lookup"><span data-stu-id="cf998-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf998-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf998-192">Request</span></span>
<span data-ttu-id="cf998-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf998-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 447

{
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cf998-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf998-194">Response</span></span>
<span data-ttu-id="cf998-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cf998-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





