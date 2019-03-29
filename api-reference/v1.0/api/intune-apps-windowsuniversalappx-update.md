---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bbd39945213b5433878b161396fee106f17a0eb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960211"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="fbb59-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="fbb59-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="fbb59-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbb59-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbb59-105">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-105">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbb59-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb59-106">Prerequisites</span></span>
<span data-ttu-id="fbb59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbb59-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb59-109">Permission type</span></span>|<span data-ttu-id="fbb59-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbb59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbb59-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbb59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbb59-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb59-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbb59-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbb59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbb59-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb59-114">Not supported.</span></span>|
|<span data-ttu-id="fbb59-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbb59-115">Application</span></span>|<span data-ttu-id="fbb59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbb59-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbb59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="fbb59-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbb59-118">Request headers</span></span>
|<span data-ttu-id="fbb59-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbb59-119">Header</span></span>|<span data-ttu-id="fbb59-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fbb59-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbb59-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbb59-121">Authorization</span></span>|<span data-ttu-id="fbb59-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbb59-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbb59-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fbb59-123">Accept</span></span>|<span data-ttu-id="fbb59-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fbb59-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbb59-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbb59-125">Request body</span></span>
<span data-ttu-id="fbb59-126">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbb59-126">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="fbb59-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-127">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="fbb59-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbb59-128">Property</span></span>|<span data-ttu-id="fbb59-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fbb59-129">Type</span></span>|<span data-ttu-id="fbb59-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb59-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbb59-131">id</span><span class="sxs-lookup"><span data-stu-id="fbb59-131">id</span></span>|<span data-ttu-id="fbb59-132">Строка</span><span class="sxs-lookup"><span data-stu-id="fbb59-132">String</span></span>|<span data-ttu-id="fbb59-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fbb59-133">Key of the entity.</span></span> <span data-ttu-id="fbb59-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fbb59-135">displayName</span></span>|<span data-ttu-id="fbb59-136">Строка</span><span class="sxs-lookup"><span data-stu-id="fbb59-136">String</span></span>|<span data-ttu-id="fbb59-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fbb59-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fbb59-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-139">description</span><span class="sxs-lookup"><span data-stu-id="fbb59-139">description</span></span>|<span data-ttu-id="fbb59-140">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-140">String</span></span>|<span data-ttu-id="fbb59-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-141">The description of the app.</span></span> <span data-ttu-id="fbb59-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-143">publisher</span><span class="sxs-lookup"><span data-stu-id="fbb59-143">publisher</span></span>|<span data-ttu-id="fbb59-144">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-144">String</span></span>|<span data-ttu-id="fbb59-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-145">The publisher of the app.</span></span> <span data-ttu-id="fbb59-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fbb59-147">largeIcon</span></span>|[<span data-ttu-id="fbb59-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fbb59-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fbb59-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fbb59-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fbb59-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb59-151">createdDateTime</span></span>|<span data-ttu-id="fbb59-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb59-152">DateTimeOffset</span></span>|<span data-ttu-id="fbb59-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-153">The date and time the app was created.</span></span> <span data-ttu-id="fbb59-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb59-155">lastModifiedDateTime</span></span>|<span data-ttu-id="fbb59-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb59-156">DateTimeOffset</span></span>|<span data-ttu-id="fbb59-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-157">The date and time the app was last modified.</span></span> <span data-ttu-id="fbb59-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fbb59-159">isFeatured</span></span>|<span data-ttu-id="fbb59-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbb59-160">Boolean</span></span>|<span data-ttu-id="fbb59-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fbb59-162">privacyInformationUrl</span></span>|<span data-ttu-id="fbb59-163">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-163">String</span></span>|<span data-ttu-id="fbb59-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fbb59-164">The privacy statement Url.</span></span> <span data-ttu-id="fbb59-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fbb59-166">informationUrl</span></span>|<span data-ttu-id="fbb59-167">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-167">String</span></span>|<span data-ttu-id="fbb59-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fbb59-168">The more information Url.</span></span> <span data-ttu-id="fbb59-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-170">owner</span><span class="sxs-lookup"><span data-stu-id="fbb59-170">owner</span></span>|<span data-ttu-id="fbb59-171">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-171">String</span></span>|<span data-ttu-id="fbb59-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-172">The owner of the app.</span></span> <span data-ttu-id="fbb59-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-174">developer</span><span class="sxs-lookup"><span data-stu-id="fbb59-174">developer</span></span>|<span data-ttu-id="fbb59-175">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-175">String</span></span>|<span data-ttu-id="fbb59-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-176">The developer of the app.</span></span> <span data-ttu-id="fbb59-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-178">notes</span><span class="sxs-lookup"><span data-stu-id="fbb59-178">notes</span></span>|<span data-ttu-id="fbb59-179">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-179">String</span></span>|<span data-ttu-id="fbb59-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-180">Notes for the app.</span></span> <span data-ttu-id="fbb59-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb59-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="fbb59-182">publishingState</span></span>|[<span data-ttu-id="fbb59-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="fbb59-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fbb59-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-184">The publishing state for the app.</span></span> <span data-ttu-id="fbb59-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fbb59-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fbb59-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fbb59-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fbb59-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fbb59-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fbb59-188">committedContentVersion</span></span>|<span data-ttu-id="fbb59-189">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-189">String</span></span>|<span data-ttu-id="fbb59-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="fbb59-190">The internal committed content version.</span></span> <span data-ttu-id="fbb59-191">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbb59-192">fileName</span><span class="sxs-lookup"><span data-stu-id="fbb59-192">fileName</span></span>|<span data-ttu-id="fbb59-193">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-193">String</span></span>|<span data-ttu-id="fbb59-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-194">The name of the main Lob application file.</span></span> <span data-ttu-id="fbb59-195">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbb59-196">size</span><span class="sxs-lookup"><span data-stu-id="fbb59-196">size</span></span>|<span data-ttu-id="fbb59-197">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb59-197">Int64</span></span>|<span data-ttu-id="fbb59-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="fbb59-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="fbb59-199">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb59-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbb59-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="fbb59-200">applicableArchitectures</span></span>|[<span data-ttu-id="fbb59-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="fbb59-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="fbb59-202">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="fbb59-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="fbb59-203">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="fbb59-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="fbb59-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="fbb59-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="fbb59-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="fbb59-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="fbb59-206">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="fbb59-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="fbb59-207">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="fbb59-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="fbb59-208">identityName</span><span class="sxs-lookup"><span data-stu-id="fbb59-208">identityName</span></span>|<span data-ttu-id="fbb59-209">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-209">String</span></span>|<span data-ttu-id="fbb59-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-210">The Identity Name.</span></span>|
|<span data-ttu-id="fbb59-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="fbb59-211">identityPublisherHash</span></span>|<span data-ttu-id="fbb59-212">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-212">String</span></span>|<span data-ttu-id="fbb59-213">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="fbb59-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="fbb59-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fbb59-214">identityResourceIdentifier</span></span>|<span data-ttu-id="fbb59-215">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-215">String</span></span>|<span data-ttu-id="fbb59-216">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="fbb59-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="fbb59-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="fbb59-217">isBundle</span></span>|<span data-ttu-id="fbb59-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbb59-218">Boolean</span></span>|<span data-ttu-id="fbb59-219">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="fbb59-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="fbb59-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbb59-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fbb59-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbb59-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="fbb59-222">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fbb59-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fbb59-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="fbb59-223">identityVersion</span></span>|<span data-ttu-id="fbb59-224">String</span><span class="sxs-lookup"><span data-stu-id="fbb59-224">String</span></span>|<span data-ttu-id="fbb59-225">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="fbb59-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="fbb59-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbb59-226">Response</span></span>
<span data-ttu-id="fbb59-227">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fbb59-227">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbb59-228">Пример</span><span class="sxs-lookup"><span data-stu-id="fbb59-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbb59-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbb59-229">Request</span></span>
<span data-ttu-id="fbb59-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbb59-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

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
  "publishingState": "processing",
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
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="fbb59-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbb59-231">Response</span></span>
<span data-ttu-id="fbb59-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbb59-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

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
  "publishingState": "processing",
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
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



