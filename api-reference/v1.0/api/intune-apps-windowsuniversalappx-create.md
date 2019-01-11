---
title: Create windowsUniversalAppX
description: Создание объекта windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d5e0a3d209b23377adfd50b4880b29c854761da3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894525"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="bc738-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="bc738-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="bc738-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc738-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc738-105">Создание объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-105">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc738-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bc738-106">Prerequisites</span></span>
<span data-ttu-id="bc738-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc738-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc738-109">Permission type</span></span>|<span data-ttu-id="bc738-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc738-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc738-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc738-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc738-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc738-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bc738-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc738-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc738-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc738-114">Not supported.</span></span>|
|<span data-ttu-id="bc738-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc738-115">Application</span></span>|<span data-ttu-id="bc738-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc738-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc738-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc738-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bc738-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc738-118">Request headers</span></span>
|<span data-ttu-id="bc738-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc738-119">Header</span></span>|<span data-ttu-id="bc738-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bc738-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc738-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc738-121">Authorization</span></span>|<span data-ttu-id="bc738-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bc738-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc738-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bc738-123">Accept</span></span>|<span data-ttu-id="bc738-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc738-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc738-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc738-125">Request body</span></span>
<span data-ttu-id="bc738-126">В тексте запроса добавьте представление объекта windowsUniversalAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc738-126">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="bc738-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="bc738-127">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="bc738-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc738-128">Property</span></span>|<span data-ttu-id="bc738-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bc738-129">Type</span></span>|<span data-ttu-id="bc738-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bc738-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc738-131">id</span><span class="sxs-lookup"><span data-stu-id="bc738-131">id</span></span>|<span data-ttu-id="bc738-132">Строка</span><span class="sxs-lookup"><span data-stu-id="bc738-132">String</span></span>|<span data-ttu-id="bc738-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc738-133">Key of the entity.</span></span> <span data-ttu-id="bc738-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bc738-135">displayName</span></span>|<span data-ttu-id="bc738-136">String</span><span class="sxs-lookup"><span data-stu-id="bc738-136">String</span></span>|<span data-ttu-id="bc738-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="bc738-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bc738-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-139">описание</span><span class="sxs-lookup"><span data-stu-id="bc738-139">description</span></span>|<span data-ttu-id="bc738-140">String</span><span class="sxs-lookup"><span data-stu-id="bc738-140">String</span></span>|<span data-ttu-id="bc738-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-141">The description of the app.</span></span> <span data-ttu-id="bc738-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-143">publisher</span><span class="sxs-lookup"><span data-stu-id="bc738-143">publisher</span></span>|<span data-ttu-id="bc738-144">String</span><span class="sxs-lookup"><span data-stu-id="bc738-144">String</span></span>|<span data-ttu-id="bc738-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-145">The publisher of the app.</span></span> <span data-ttu-id="bc738-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bc738-147">largeIcon</span></span>|[<span data-ttu-id="bc738-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bc738-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bc738-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="bc738-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bc738-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc738-151">createdDateTime</span></span>|<span data-ttu-id="bc738-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc738-152">DateTimeOffset</span></span>|<span data-ttu-id="bc738-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-153">The date and time the app was created.</span></span> <span data-ttu-id="bc738-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc738-155">lastModifiedDateTime</span></span>|<span data-ttu-id="bc738-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc738-156">DateTimeOffset</span></span>|<span data-ttu-id="bc738-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-157">The date and time the app was last modified.</span></span> <span data-ttu-id="bc738-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bc738-159">isFeatured</span></span>|<span data-ttu-id="bc738-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc738-160">Boolean</span></span>|<span data-ttu-id="bc738-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bc738-162">privacyInformationUrl</span></span>|<span data-ttu-id="bc738-163">String</span><span class="sxs-lookup"><span data-stu-id="bc738-163">String</span></span>|<span data-ttu-id="bc738-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="bc738-164">The privacy statement Url.</span></span> <span data-ttu-id="bc738-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bc738-166">informationUrl</span></span>|<span data-ttu-id="bc738-167">String</span><span class="sxs-lookup"><span data-stu-id="bc738-167">String</span></span>|<span data-ttu-id="bc738-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="bc738-168">The more information Url.</span></span> <span data-ttu-id="bc738-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-170">owner</span><span class="sxs-lookup"><span data-stu-id="bc738-170">owner</span></span>|<span data-ttu-id="bc738-171">String</span><span class="sxs-lookup"><span data-stu-id="bc738-171">String</span></span>|<span data-ttu-id="bc738-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-172">The owner of the app.</span></span> <span data-ttu-id="bc738-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-174">developer</span><span class="sxs-lookup"><span data-stu-id="bc738-174">developer</span></span>|<span data-ttu-id="bc738-175">String</span><span class="sxs-lookup"><span data-stu-id="bc738-175">String</span></span>|<span data-ttu-id="bc738-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-176">The developer of the app.</span></span> <span data-ttu-id="bc738-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-178">notes</span><span class="sxs-lookup"><span data-stu-id="bc738-178">notes</span></span>|<span data-ttu-id="bc738-179">String</span><span class="sxs-lookup"><span data-stu-id="bc738-179">String</span></span>|<span data-ttu-id="bc738-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="bc738-180">Notes for the app.</span></span> <span data-ttu-id="bc738-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc738-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="bc738-182">publishingState</span></span>|[<span data-ttu-id="bc738-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bc738-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bc738-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-184">The publishing state for the app.</span></span> <span data-ttu-id="bc738-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="bc738-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bc738-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bc738-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bc738-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bc738-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bc738-188">committedContentVersion</span></span>|<span data-ttu-id="bc738-189">String</span><span class="sxs-lookup"><span data-stu-id="bc738-189">String</span></span>|<span data-ttu-id="bc738-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="bc738-190">The internal committed content version.</span></span> <span data-ttu-id="bc738-191">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc738-192">fileName</span><span class="sxs-lookup"><span data-stu-id="bc738-192">fileName</span></span>|<span data-ttu-id="bc738-193">String</span><span class="sxs-lookup"><span data-stu-id="bc738-193">String</span></span>|<span data-ttu-id="bc738-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="bc738-194">The name of the main Lob application file.</span></span> <span data-ttu-id="bc738-195">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc738-196">size</span><span class="sxs-lookup"><span data-stu-id="bc738-196">size</span></span>|<span data-ttu-id="bc738-197">Int64</span><span class="sxs-lookup"><span data-stu-id="bc738-197">Int64</span></span>|<span data-ttu-id="bc738-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="bc738-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="bc738-199">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc738-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc738-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="bc738-200">applicableArchitectures</span></span>|[<span data-ttu-id="bc738-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="bc738-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="bc738-202">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="bc738-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="bc738-203">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="bc738-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="bc738-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="bc738-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="bc738-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="bc738-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="bc738-206">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="bc738-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="bc738-207">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="bc738-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="bc738-208">identityName</span><span class="sxs-lookup"><span data-stu-id="bc738-208">identityName</span></span>|<span data-ttu-id="bc738-209">String</span><span class="sxs-lookup"><span data-stu-id="bc738-209">String</span></span>|<span data-ttu-id="bc738-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bc738-210">The Identity Name.</span></span>|
|<span data-ttu-id="bc738-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="bc738-211">identityPublisherHash</span></span>|<span data-ttu-id="bc738-212">String</span><span class="sxs-lookup"><span data-stu-id="bc738-212">String</span></span>|<span data-ttu-id="bc738-213">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="bc738-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="bc738-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc738-214">identityResourceIdentifier</span></span>|<span data-ttu-id="bc738-215">String</span><span class="sxs-lookup"><span data-stu-id="bc738-215">String</span></span>|<span data-ttu-id="bc738-216">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="bc738-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="bc738-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="bc738-217">isBundle</span></span>|<span data-ttu-id="bc738-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc738-218">Boolean</span></span>|<span data-ttu-id="bc738-219">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="bc738-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="bc738-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc738-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bc738-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc738-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="bc738-222">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="bc738-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bc738-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bc738-223">identityVersion</span></span>|<span data-ttu-id="bc738-224">String</span><span class="sxs-lookup"><span data-stu-id="bc738-224">String</span></span>|<span data-ttu-id="bc738-225">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bc738-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="bc738-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc738-226">Response</span></span>
<span data-ttu-id="bc738-227">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bc738-227">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc738-228">Пример</span><span class="sxs-lookup"><span data-stu-id="bc738-228">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc738-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc738-229">Request</span></span>
<span data-ttu-id="bc738-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc738-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc738-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc738-231">Response</span></span>
<span data-ttu-id="bc738-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc738-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



