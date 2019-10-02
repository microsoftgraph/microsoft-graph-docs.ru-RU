---
title: Create windowsUniversalAppX
description: Создание объекта windowsUniversalAppX.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05bf490b9352a8da29348896bf0fe06c13950875
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354933"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="d0caf-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="d0caf-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="d0caf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0caf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0caf-105">Создание объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-105">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0caf-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d0caf-106">Prerequisites</span></span>
<span data-ttu-id="d0caf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0caf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0caf-109">Permission type</span></span>|<span data-ttu-id="d0caf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0caf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0caf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0caf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0caf-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0caf-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d0caf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0caf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0caf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0caf-114">Not supported.</span></span>|
|<span data-ttu-id="d0caf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0caf-115">Application</span></span>|<span data-ttu-id="d0caf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0caf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0caf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0caf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d0caf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0caf-118">Request headers</span></span>
|<span data-ttu-id="d0caf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0caf-119">Header</span></span>|<span data-ttu-id="d0caf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d0caf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0caf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0caf-121">Authorization</span></span>|<span data-ttu-id="d0caf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0caf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0caf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d0caf-123">Accept</span></span>|<span data-ttu-id="d0caf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0caf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0caf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0caf-125">Request body</span></span>
<span data-ttu-id="d0caf-126">В тексте запроса добавьте представление объекта windowsUniversalAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0caf-126">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="d0caf-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="d0caf-127">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="d0caf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0caf-128">Property</span></span>|<span data-ttu-id="d0caf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d0caf-129">Type</span></span>|<span data-ttu-id="d0caf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d0caf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0caf-131">id</span><span class="sxs-lookup"><span data-stu-id="d0caf-131">id</span></span>|<span data-ttu-id="d0caf-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d0caf-132">String</span></span>|<span data-ttu-id="d0caf-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0caf-133">Key of the entity.</span></span> <span data-ttu-id="d0caf-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d0caf-135">displayName</span></span>|<span data-ttu-id="d0caf-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d0caf-136">String</span></span>|<span data-ttu-id="d0caf-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d0caf-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d0caf-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-139">description</span><span class="sxs-lookup"><span data-stu-id="d0caf-139">description</span></span>|<span data-ttu-id="d0caf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d0caf-140">String</span></span>|<span data-ttu-id="d0caf-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-141">The description of the app.</span></span> <span data-ttu-id="d0caf-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-143">publisher</span><span class="sxs-lookup"><span data-stu-id="d0caf-143">publisher</span></span>|<span data-ttu-id="d0caf-144">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-144">String</span></span>|<span data-ttu-id="d0caf-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-145">The publisher of the app.</span></span> <span data-ttu-id="d0caf-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d0caf-147">largeIcon</span></span>|[<span data-ttu-id="d0caf-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d0caf-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d0caf-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d0caf-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d0caf-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0caf-151">createdDateTime</span></span>|<span data-ttu-id="d0caf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0caf-152">DateTimeOffset</span></span>|<span data-ttu-id="d0caf-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-153">The date and time the app was created.</span></span> <span data-ttu-id="d0caf-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0caf-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d0caf-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0caf-156">DateTimeOffset</span></span>|<span data-ttu-id="d0caf-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-157">The date and time the app was last modified.</span></span> <span data-ttu-id="d0caf-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d0caf-159">isFeatured</span></span>|<span data-ttu-id="d0caf-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0caf-160">Boolean</span></span>|<span data-ttu-id="d0caf-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d0caf-162">privacyInformationUrl</span></span>|<span data-ttu-id="d0caf-163">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-163">String</span></span>|<span data-ttu-id="d0caf-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d0caf-164">The privacy statement Url.</span></span> <span data-ttu-id="d0caf-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d0caf-166">informationUrl</span></span>|<span data-ttu-id="d0caf-167">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-167">String</span></span>|<span data-ttu-id="d0caf-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d0caf-168">The more information Url.</span></span> <span data-ttu-id="d0caf-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-170">owner</span><span class="sxs-lookup"><span data-stu-id="d0caf-170">owner</span></span>|<span data-ttu-id="d0caf-171">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-171">String</span></span>|<span data-ttu-id="d0caf-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-172">The owner of the app.</span></span> <span data-ttu-id="d0caf-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-174">developer</span><span class="sxs-lookup"><span data-stu-id="d0caf-174">developer</span></span>|<span data-ttu-id="d0caf-175">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-175">String</span></span>|<span data-ttu-id="d0caf-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-176">The developer of the app.</span></span> <span data-ttu-id="d0caf-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-178">notes</span><span class="sxs-lookup"><span data-stu-id="d0caf-178">notes</span></span>|<span data-ttu-id="d0caf-179">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-179">String</span></span>|<span data-ttu-id="d0caf-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-180">Notes for the app.</span></span> <span data-ttu-id="d0caf-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d0caf-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="d0caf-182">publishingState</span></span>|[<span data-ttu-id="d0caf-183">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d0caf-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d0caf-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-184">The publishing state for the app.</span></span> <span data-ttu-id="d0caf-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d0caf-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d0caf-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d0caf-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d0caf-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d0caf-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d0caf-188">committedContentVersion</span></span>|<span data-ttu-id="d0caf-189">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-189">String</span></span>|<span data-ttu-id="d0caf-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="d0caf-190">The internal committed content version.</span></span> <span data-ttu-id="d0caf-191">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d0caf-192">fileName</span><span class="sxs-lookup"><span data-stu-id="d0caf-192">fileName</span></span>|<span data-ttu-id="d0caf-193">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-193">String</span></span>|<span data-ttu-id="d0caf-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-194">The name of the main Lob application file.</span></span> <span data-ttu-id="d0caf-195">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d0caf-196">size</span><span class="sxs-lookup"><span data-stu-id="d0caf-196">size</span></span>|<span data-ttu-id="d0caf-197">Int64</span><span class="sxs-lookup"><span data-stu-id="d0caf-197">Int64</span></span>|<span data-ttu-id="d0caf-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="d0caf-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="d0caf-199">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0caf-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d0caf-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="d0caf-200">applicableArchitectures</span></span>|[<span data-ttu-id="d0caf-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="d0caf-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="d0caf-202">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="d0caf-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="d0caf-203">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="d0caf-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="d0caf-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="d0caf-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="d0caf-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="d0caf-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="d0caf-206">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="d0caf-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="d0caf-207">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="d0caf-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="d0caf-208">identityName</span><span class="sxs-lookup"><span data-stu-id="d0caf-208">identityName</span></span>|<span data-ttu-id="d0caf-209">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-209">String</span></span>|<span data-ttu-id="d0caf-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-210">The Identity Name.</span></span>|
|<span data-ttu-id="d0caf-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="d0caf-211">identityPublisherHash</span></span>|<span data-ttu-id="d0caf-212">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-212">String</span></span>|<span data-ttu-id="d0caf-213">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d0caf-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="d0caf-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d0caf-214">identityResourceIdentifier</span></span>|<span data-ttu-id="d0caf-215">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-215">String</span></span>|<span data-ttu-id="d0caf-216">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="d0caf-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="d0caf-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="d0caf-217">isBundle</span></span>|<span data-ttu-id="d0caf-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0caf-218">Boolean</span></span>|<span data-ttu-id="d0caf-219">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="d0caf-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="d0caf-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d0caf-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d0caf-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d0caf-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="d0caf-222">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d0caf-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d0caf-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d0caf-223">identityVersion</span></span>|<span data-ttu-id="d0caf-224">String</span><span class="sxs-lookup"><span data-stu-id="d0caf-224">String</span></span>|<span data-ttu-id="d0caf-225">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d0caf-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d0caf-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0caf-226">Response</span></span>
<span data-ttu-id="d0caf-227">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d0caf-227">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0caf-228">Пример</span><span class="sxs-lookup"><span data-stu-id="d0caf-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0caf-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0caf-229">Request</span></span>
<span data-ttu-id="d0caf-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0caf-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="d0caf-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0caf-231">Response</span></span>
<span data-ttu-id="d0caf-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0caf-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




