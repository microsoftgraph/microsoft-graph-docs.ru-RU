---
title: Create windowsUniversalAppX
description: Создание объекта windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bdbab2d23d3777e72aa291a9729f0480793883f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149772"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="38197-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="38197-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="38197-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38197-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38197-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38197-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38197-106">Создание объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="38197-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38197-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="38197-107">Prerequisites</span></span>
<span data-ttu-id="38197-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="38197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="38197-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38197-110">Permission type</span></span>|<span data-ttu-id="38197-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38197-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38197-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38197-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38197-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38197-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38197-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38197-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38197-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38197-115">Not supported.</span></span>|
|<span data-ttu-id="38197-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38197-116">Application</span></span>|<span data-ttu-id="38197-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38197-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38197-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38197-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="38197-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38197-119">Request headers</span></span>
|<span data-ttu-id="38197-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38197-120">Header</span></span>|<span data-ttu-id="38197-121">Значение</span><span class="sxs-lookup"><span data-stu-id="38197-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38197-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38197-122">Authorization</span></span>|<span data-ttu-id="38197-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="38197-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38197-124">Accept</span><span class="sxs-lookup"><span data-stu-id="38197-124">Accept</span></span>|<span data-ttu-id="38197-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38197-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38197-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38197-126">Request body</span></span>
<span data-ttu-id="38197-127">В тексте запроса добавьте представление объекта windowsUniversalAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38197-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="38197-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="38197-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="38197-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="38197-129">Property</span></span>|<span data-ttu-id="38197-130">Тип</span><span class="sxs-lookup"><span data-stu-id="38197-130">Type</span></span>|<span data-ttu-id="38197-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38197-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38197-132">id</span><span class="sxs-lookup"><span data-stu-id="38197-132">id</span></span>|<span data-ttu-id="38197-133">Строка</span><span class="sxs-lookup"><span data-stu-id="38197-133">String</span></span>|<span data-ttu-id="38197-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38197-134">Key of the entity.</span></span> <span data-ttu-id="38197-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-136">displayName</span><span class="sxs-lookup"><span data-stu-id="38197-136">displayName</span></span>|<span data-ttu-id="38197-137">String</span><span class="sxs-lookup"><span data-stu-id="38197-137">String</span></span>|<span data-ttu-id="38197-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="38197-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="38197-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-140">description</span><span class="sxs-lookup"><span data-stu-id="38197-140">description</span></span>|<span data-ttu-id="38197-141">Строка</span><span class="sxs-lookup"><span data-stu-id="38197-141">String</span></span>|<span data-ttu-id="38197-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-142">The description of the app.</span></span> <span data-ttu-id="38197-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-144">publisher</span><span class="sxs-lookup"><span data-stu-id="38197-144">publisher</span></span>|<span data-ttu-id="38197-145">String</span><span class="sxs-lookup"><span data-stu-id="38197-145">String</span></span>|<span data-ttu-id="38197-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-146">The publisher of the app.</span></span> <span data-ttu-id="38197-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="38197-148">largeIcon</span></span>|[<span data-ttu-id="38197-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="38197-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="38197-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="38197-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="38197-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38197-152">createdDateTime</span></span>|<span data-ttu-id="38197-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38197-153">DateTimeOffset</span></span>|<span data-ttu-id="38197-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-154">The date and time the app was created.</span></span> <span data-ttu-id="38197-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38197-156">lastModifiedDateTime</span></span>|<span data-ttu-id="38197-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38197-157">DateTimeOffset</span></span>|<span data-ttu-id="38197-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-158">The date and time the app was last modified.</span></span> <span data-ttu-id="38197-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="38197-160">isFeatured</span></span>|<span data-ttu-id="38197-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="38197-161">Boolean</span></span>|<span data-ttu-id="38197-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="38197-163">privacyInformationUrl</span></span>|<span data-ttu-id="38197-164">String</span><span class="sxs-lookup"><span data-stu-id="38197-164">String</span></span>|<span data-ttu-id="38197-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="38197-165">The privacy statement Url.</span></span> <span data-ttu-id="38197-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="38197-167">informationUrl</span></span>|<span data-ttu-id="38197-168">String</span><span class="sxs-lookup"><span data-stu-id="38197-168">String</span></span>|<span data-ttu-id="38197-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="38197-169">The more information Url.</span></span> <span data-ttu-id="38197-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-171">owner</span><span class="sxs-lookup"><span data-stu-id="38197-171">owner</span></span>|<span data-ttu-id="38197-172">Строка</span><span class="sxs-lookup"><span data-stu-id="38197-172">String</span></span>|<span data-ttu-id="38197-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-173">The owner of the app.</span></span> <span data-ttu-id="38197-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-175">developer</span><span class="sxs-lookup"><span data-stu-id="38197-175">developer</span></span>|<span data-ttu-id="38197-176">String</span><span class="sxs-lookup"><span data-stu-id="38197-176">String</span></span>|<span data-ttu-id="38197-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-177">The developer of the app.</span></span> <span data-ttu-id="38197-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-179">notes</span><span class="sxs-lookup"><span data-stu-id="38197-179">notes</span></span>|<span data-ttu-id="38197-180">String</span><span class="sxs-lookup"><span data-stu-id="38197-180">String</span></span>|<span data-ttu-id="38197-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="38197-181">Notes for the app.</span></span> <span data-ttu-id="38197-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="38197-183">uploadState</span></span>|<span data-ttu-id="38197-184">Int32</span><span class="sxs-lookup"><span data-stu-id="38197-184">Int32</span></span>|<span data-ttu-id="38197-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="38197-185">The upload state.</span></span> <span data-ttu-id="38197-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="38197-187">publishingState</span></span>|[<span data-ttu-id="38197-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="38197-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="38197-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-189">The publishing state for the app.</span></span> <span data-ttu-id="38197-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="38197-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="38197-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="38197-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="38197-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="38197-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="38197-193">isAssigned</span></span>|<span data-ttu-id="38197-194">Логический</span><span class="sxs-lookup"><span data-stu-id="38197-194">Boolean</span></span>|<span data-ttu-id="38197-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="38197-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="38197-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38197-197">roleScopeTagIds</span></span>|<span data-ttu-id="38197-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="38197-198">String collection</span></span>|<span data-ttu-id="38197-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="38197-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="38197-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="38197-201">committedContentVersion</span></span>|<span data-ttu-id="38197-202">String</span><span class="sxs-lookup"><span data-stu-id="38197-202">String</span></span>|<span data-ttu-id="38197-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="38197-203">The internal committed content version.</span></span> <span data-ttu-id="38197-204">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="38197-205">fileName</span><span class="sxs-lookup"><span data-stu-id="38197-205">fileName</span></span>|<span data-ttu-id="38197-206">String</span><span class="sxs-lookup"><span data-stu-id="38197-206">String</span></span>|<span data-ttu-id="38197-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="38197-207">The name of the main Lob application file.</span></span> <span data-ttu-id="38197-208">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="38197-209">size</span><span class="sxs-lookup"><span data-stu-id="38197-209">size</span></span>|<span data-ttu-id="38197-210">Int64</span><span class="sxs-lookup"><span data-stu-id="38197-210">Int64</span></span>|<span data-ttu-id="38197-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="38197-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="38197-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="38197-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="38197-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="38197-213">applicableArchitectures</span></span>|[<span data-ttu-id="38197-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="38197-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="38197-215">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="38197-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="38197-216">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="38197-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="38197-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="38197-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="38197-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="38197-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="38197-219">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="38197-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="38197-220">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="38197-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="38197-221">identityName</span><span class="sxs-lookup"><span data-stu-id="38197-221">identityName</span></span>|<span data-ttu-id="38197-222">String</span><span class="sxs-lookup"><span data-stu-id="38197-222">String</span></span>|<span data-ttu-id="38197-223">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="38197-223">The Identity Name.</span></span>|
|<span data-ttu-id="38197-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="38197-224">identityPublisherHash</span></span>|<span data-ttu-id="38197-225">String</span><span class="sxs-lookup"><span data-stu-id="38197-225">String</span></span>|<span data-ttu-id="38197-226">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="38197-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="38197-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="38197-227">identityResourceIdentifier</span></span>|<span data-ttu-id="38197-228">String</span><span class="sxs-lookup"><span data-stu-id="38197-228">String</span></span>|<span data-ttu-id="38197-229">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="38197-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="38197-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="38197-230">isBundle</span></span>|<span data-ttu-id="38197-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="38197-231">Boolean</span></span>|<span data-ttu-id="38197-232">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="38197-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="38197-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="38197-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="38197-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="38197-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="38197-235">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="38197-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="38197-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="38197-236">identityVersion</span></span>|<span data-ttu-id="38197-237">String</span><span class="sxs-lookup"><span data-stu-id="38197-237">String</span></span>|<span data-ttu-id="38197-238">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="38197-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="38197-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="38197-239">Response</span></span>
<span data-ttu-id="38197-240">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="38197-240">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38197-241">Пример</span><span class="sxs-lookup"><span data-stu-id="38197-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="38197-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="38197-242">Request</span></span>
<span data-ttu-id="38197-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38197-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1388

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="38197-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="38197-244">Response</span></span>
<span data-ttu-id="38197-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38197-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1560

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```




