---
title: Обновление networkIPv4ConfigurationManagementCondition
description: Обновление свойства объекта networkIPv4ConfigurationManagementCondition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ba949cacb4bdfe26de809f3baeaaece68918eab9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402085"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="bc47d-103">Обновление networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="bc47d-103">Update networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="bc47d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc47d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc47d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc47d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc47d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc47d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc47d-107">Обновление свойства объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="bc47d-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc47d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bc47d-108">Prerequisites</span></span>
<span data-ttu-id="bc47d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc47d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc47d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc47d-111">Permission type</span></span>|<span data-ttu-id="bc47d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc47d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc47d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc47d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc47d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc47d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc47d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc47d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc47d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc47d-116">Not supported.</span></span>|
|<span data-ttu-id="bc47d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc47d-117">Application</span></span>|<span data-ttu-id="bc47d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc47d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc47d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc47d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="bc47d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc47d-120">Request headers</span></span>
|<span data-ttu-id="bc47d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc47d-121">Header</span></span>|<span data-ttu-id="bc47d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bc47d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc47d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc47d-123">Authorization</span></span>|<span data-ttu-id="bc47d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bc47d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc47d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc47d-125">Accept</span></span>|<span data-ttu-id="bc47d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc47d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc47d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc47d-127">Request body</span></span>
<span data-ttu-id="bc47d-128">В тексте запроса укажите представление JSON для объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="bc47d-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="bc47d-129">В следующей таблице показаны свойства, которые необходимы для создания [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="bc47d-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="bc47d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc47d-130">Property</span></span>|<span data-ttu-id="bc47d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc47d-131">Type</span></span>|<span data-ttu-id="bc47d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc47d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc47d-133">id</span><span class="sxs-lookup"><span data-stu-id="bc47d-133">id</span></span>|<span data-ttu-id="bc47d-134">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-134">String</span></span>|<span data-ttu-id="bc47d-135">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="bc47d-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="bc47d-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="bc47d-136">System generated value assigned when created.</span></span> <span data-ttu-id="bc47d-137">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-138">уникального имени</span><span class="sxs-lookup"><span data-stu-id="bc47d-138">uniqueName</span></span>|<span data-ttu-id="bc47d-139">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-139">String</span></span>|<span data-ttu-id="bc47d-140">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="bc47d-140">Unique name for the management condition.</span></span> <span data-ttu-id="bc47d-141">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="bc47d-141">Used in management condition expressions.</span></span> <span data-ttu-id="bc47d-142">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="bc47d-143">displayName</span></span>|<span data-ttu-id="bc47d-144">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-144">String</span></span>|<span data-ttu-id="bc47d-145">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="bc47d-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="bc47d-146">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-147">description</span><span class="sxs-lookup"><span data-stu-id="bc47d-147">description</span></span>|<span data-ttu-id="bc47d-148">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-148">String</span></span>|<span data-ttu-id="bc47d-149">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="bc47d-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="bc47d-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc47d-151">createdDateTime</span></span>|<span data-ttu-id="bc47d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc47d-152">DateTimeOffset</span></span>|<span data-ttu-id="bc47d-153">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="bc47d-153">The time the management condition was created.</span></span> <span data-ttu-id="bc47d-154">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="bc47d-154">Generated service side.</span></span> <span data-ttu-id="bc47d-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc47d-156">modifiedDateTime</span></span>|<span data-ttu-id="bc47d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc47d-157">DateTimeOffset</span></span>|<span data-ttu-id="bc47d-158">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="bc47d-158">The time the management condition was last modified.</span></span> <span data-ttu-id="bc47d-159">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="bc47d-159">Updated service side.</span></span> <span data-ttu-id="bc47d-160">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-161">eTag</span><span class="sxs-lookup"><span data-stu-id="bc47d-161">eTag</span></span>|<span data-ttu-id="bc47d-162">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-162">String</span></span>|<span data-ttu-id="bc47d-163">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="bc47d-163">ETag of the management condition.</span></span> <span data-ttu-id="bc47d-164">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="bc47d-164">Updated service side.</span></span> <span data-ttu-id="bc47d-165">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bc47d-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bc47d-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="bc47d-166">applicablePlatforms</span></span>|<span data-ttu-id="bc47d-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bc47d-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="bc47d-168">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="bc47d-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="bc47d-169">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="bc47d-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="bc47d-170">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="bc47d-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="bc47d-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="bc47d-171">ipV4Prefix</span></span>|<span data-ttu-id="bc47d-172">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-172">String</span></span>|<span data-ttu-id="bc47d-173">Подсеть IPv4, подключенных к.</span><span class="sxs-lookup"><span data-stu-id="bc47d-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="bc47d-174">например 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="bc47d-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="bc47d-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="bc47d-175">ipV4Gateway</span></span>|<span data-ttu-id="bc47d-176">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-176">String</span></span>|<span data-ttu-id="bc47d-177">IPv4-адрес шлюза.</span><span class="sxs-lookup"><span data-stu-id="bc47d-177">The IPv4 gateway address.</span></span> <span data-ttu-id="bc47d-178">например 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="bc47d-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="bc47d-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="bc47d-179">ipV4DHCPServer</span></span>|<span data-ttu-id="bc47d-180">String</span><span class="sxs-lookup"><span data-stu-id="bc47d-180">String</span></span>|<span data-ttu-id="bc47d-181">IPv4-адрес на DHCP-сервер для адаптера.</span><span class="sxs-lookup"><span data-stu-id="bc47d-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="bc47d-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="bc47d-182">ipV4DNSServerList</span></span>|<span data-ttu-id="bc47d-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc47d-183">String collection</span></span>|<span data-ttu-id="bc47d-184">IPv4 DNS-серверов, настроенных для адаптера.</span><span class="sxs-lookup"><span data-stu-id="bc47d-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="bc47d-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="bc47d-185">dnsSuffixList</span></span>|<span data-ttu-id="bc47d-186">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc47d-186">String collection</span></span>|<span data-ttu-id="bc47d-187">Допустимое DNS-суффиксы для текущей сети.</span><span class="sxs-lookup"><span data-stu-id="bc47d-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="bc47d-188">Например seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="bc47d-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="bc47d-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc47d-189">Response</span></span>
<span data-ttu-id="bc47d-190">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc47d-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc47d-191">Пример</span><span class="sxs-lookup"><span data-stu-id="bc47d-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc47d-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc47d-192">Request</span></span>
<span data-ttu-id="bc47d-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc47d-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
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

### <a name="response"></a><span data-ttu-id="bc47d-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc47d-194">Response</span></span>
<span data-ttu-id="bc47d-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc47d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




