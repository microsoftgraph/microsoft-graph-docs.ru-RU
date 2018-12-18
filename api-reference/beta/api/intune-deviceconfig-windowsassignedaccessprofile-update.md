---
title: Обновление windowsAssignedAccessProfile
description: Обновление свойства объекта windowsAssignedAccessProfile.
author: tfitzmac
ms.openlocfilehash: 84cbc1aaaebf9383c3d113d7f309c61de0cdeb67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331362"
---
# <a name="update-windowsassignedaccessprofile"></a><span data-ttu-id="736d1-103">Обновление windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="736d1-103">Update windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="736d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="736d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="736d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="736d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="736d1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="736d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="736d1-107">Обновление свойства объекта [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="736d1-107">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="736d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="736d1-108">Prerequisites</span></span>
<span data-ttu-id="736d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="736d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="736d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="736d1-111">Permission type</span></span>|<span data-ttu-id="736d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="736d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="736d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="736d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="736d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="736d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="736d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="736d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="736d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="736d1-116">Not supported.</span></span>|
|<span data-ttu-id="736d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="736d1-117">Application</span></span>|<span data-ttu-id="736d1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="736d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="736d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="736d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="736d1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="736d1-120">Request headers</span></span>
|<span data-ttu-id="736d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="736d1-121">Header</span></span>|<span data-ttu-id="736d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="736d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="736d1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="736d1-123">Authorization</span></span>|<span data-ttu-id="736d1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="736d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="736d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="736d1-125">Accept</span></span>|<span data-ttu-id="736d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="736d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="736d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="736d1-127">Request body</span></span>
<span data-ttu-id="736d1-128">В тексте запроса укажите представление JSON для объекта [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="736d1-128">In the request body, supply a JSON representation for the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>

<span data-ttu-id="736d1-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span><span class="sxs-lookup"><span data-stu-id="736d1-129">The following table shows the properties that are required when you create the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>

|<span data-ttu-id="736d1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="736d1-130">Property</span></span>|<span data-ttu-id="736d1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="736d1-131">Type</span></span>|<span data-ttu-id="736d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="736d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="736d1-133">id</span><span class="sxs-lookup"><span data-stu-id="736d1-133">id</span></span>|<span data-ttu-id="736d1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="736d1-134">String</span></span>|<span data-ttu-id="736d1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="736d1-135">Key of the entity.</span></span>|
|<span data-ttu-id="736d1-136">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="736d1-136">profileName</span></span>|<span data-ttu-id="736d1-137">String.</span><span class="sxs-lookup"><span data-stu-id="736d1-137">String</span></span>|<span data-ttu-id="736d1-138">Это понятное имя, используемое для идентификации групп приложений, макет эти приложения в меню Пуск и пользователи, которым назначена эта конфигурация киоска.</span><span class="sxs-lookup"><span data-stu-id="736d1-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="736d1-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="736d1-139">showTaskBar</span></span>|<span data-ttu-id="736d1-140">Boolean.</span><span class="sxs-lookup"><span data-stu-id="736d1-140">Boolean</span></span>|<span data-ttu-id="736d1-141">Этот параметр позволяет администратору задать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="736d1-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="736d1-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="736d1-142">appUserModelIds</span></span>|<span data-ttu-id="736d1-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="736d1-143">String collection</span></span>|<span data-ttu-id="736d1-144">Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск.</span><span class="sxs-lookup"><span data-stu-id="736d1-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="736d1-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="736d1-145">desktopAppPaths</span></span>|<span data-ttu-id="736d1-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="736d1-146">String collection</span></span>|<span data-ttu-id="736d1-147">Ниже приведены пути в настольных приложений, которые будут доступны в меню Пуск и только приложения пользователь будет иметь возможность запуска.</span><span class="sxs-lookup"><span data-stu-id="736d1-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="736d1-148">userAccounts</span><span class="sxs-lookup"><span data-stu-id="736d1-148">userAccounts</span></span>|<span data-ttu-id="736d1-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="736d1-149">String collection</span></span>|<span data-ttu-id="736d1-150">Учетные записи пользователей, которые будут заблокированы для этой базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="736d1-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="736d1-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="736d1-151">startMenuLayoutXml</span></span>|<span data-ttu-id="736d1-152">Binary</span><span class="sxs-lookup"><span data-stu-id="736d1-152">Binary</span></span>|<span data-ttu-id="736d1-153">Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="736d1-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="736d1-154">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="736d1-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="736d1-155">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="736d1-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="736d1-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="736d1-156">Response</span></span>
<span data-ttu-id="736d1-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="736d1-157">If successful, this method returns a `200 OK` response code and an updated [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="736d1-158">Пример</span><span class="sxs-lookup"><span data-stu-id="736d1-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="736d1-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="736d1-159">Request</span></span>
<span data-ttu-id="736d1-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="736d1-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
Content-type: application/json
Content-length: 297

{
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a><span data-ttu-id="736d1-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="736d1-161">Response</span></span>
<span data-ttu-id="736d1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="736d1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





