---
title: Update iosLobApp
description: Обновление свойств объекта iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97227b572d22adf59f8414309d6840ce60096530
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259593"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="c3d19-103">Update iosLobApp</span><span class="sxs-lookup"><span data-stu-id="c3d19-103">Update iosLobApp</span></span>

> <span data-ttu-id="c3d19-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3d19-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3d19-105">Обновление свойств объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-105">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3d19-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d19-106">Prerequisites</span></span>
<span data-ttu-id="c3d19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c3d19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d19-109">Permission type</span></span>|<span data-ttu-id="c3d19-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3d19-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3d19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3d19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3d19-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3d19-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3d19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3d19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3d19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d19-114">Not supported.</span></span>|
|<span data-ttu-id="c3d19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3d19-115">Application</span></span>|<span data-ttu-id="c3d19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3d19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3d19-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c3d19-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3d19-118">Request headers</span></span>
|<span data-ttu-id="c3d19-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3d19-119">Header</span></span>|<span data-ttu-id="c3d19-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c3d19-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3d19-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3d19-121">Authorization</span></span>|<span data-ttu-id="c3d19-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c3d19-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3d19-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c3d19-123">Accept</span></span>|<span data-ttu-id="c3d19-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3d19-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3d19-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3d19-125">Request body</span></span>
<span data-ttu-id="c3d19-126">В теле запроса добавьте представление объекта [iosLobApp](../resources/intune-apps-ioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3d19-126">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="c3d19-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-127">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="c3d19-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3d19-128">Property</span></span>|<span data-ttu-id="c3d19-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c3d19-129">Type</span></span>|<span data-ttu-id="c3d19-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c3d19-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3d19-131">id</span><span class="sxs-lookup"><span data-stu-id="c3d19-131">id</span></span>|<span data-ttu-id="c3d19-132">Строка</span><span class="sxs-lookup"><span data-stu-id="c3d19-132">String</span></span>|<span data-ttu-id="c3d19-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3d19-133">Key of the entity.</span></span> <span data-ttu-id="c3d19-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c3d19-135">displayName</span></span>|<span data-ttu-id="c3d19-136">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-136">String</span></span>|<span data-ttu-id="c3d19-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c3d19-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c3d19-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-139">description</span><span class="sxs-lookup"><span data-stu-id="c3d19-139">description</span></span>|<span data-ttu-id="c3d19-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c3d19-140">String</span></span>|<span data-ttu-id="c3d19-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-141">The description of the app.</span></span> <span data-ttu-id="c3d19-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-143">publisher</span><span class="sxs-lookup"><span data-stu-id="c3d19-143">publisher</span></span>|<span data-ttu-id="c3d19-144">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-144">String</span></span>|<span data-ttu-id="c3d19-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-145">The publisher of the app.</span></span> <span data-ttu-id="c3d19-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c3d19-147">largeIcon</span></span>|[<span data-ttu-id="c3d19-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c3d19-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c3d19-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c3d19-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c3d19-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3d19-151">createdDateTime</span></span>|<span data-ttu-id="c3d19-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3d19-152">DateTimeOffset</span></span>|<span data-ttu-id="c3d19-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-153">The date and time the app was created.</span></span> <span data-ttu-id="c3d19-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3d19-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c3d19-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3d19-156">DateTimeOffset</span></span>|<span data-ttu-id="c3d19-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-157">The date and time the app was last modified.</span></span> <span data-ttu-id="c3d19-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c3d19-159">isFeatured</span></span>|<span data-ttu-id="c3d19-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3d19-160">Boolean</span></span>|<span data-ttu-id="c3d19-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c3d19-162">privacyInformationUrl</span></span>|<span data-ttu-id="c3d19-163">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-163">String</span></span>|<span data-ttu-id="c3d19-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c3d19-164">The privacy statement Url.</span></span> <span data-ttu-id="c3d19-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c3d19-166">informationUrl</span></span>|<span data-ttu-id="c3d19-167">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-167">String</span></span>|<span data-ttu-id="c3d19-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c3d19-168">The more information Url.</span></span> <span data-ttu-id="c3d19-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-170">owner</span><span class="sxs-lookup"><span data-stu-id="c3d19-170">owner</span></span>|<span data-ttu-id="c3d19-171">Строка</span><span class="sxs-lookup"><span data-stu-id="c3d19-171">String</span></span>|<span data-ttu-id="c3d19-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-172">The owner of the app.</span></span> <span data-ttu-id="c3d19-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-174">developer</span><span class="sxs-lookup"><span data-stu-id="c3d19-174">developer</span></span>|<span data-ttu-id="c3d19-175">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-175">String</span></span>|<span data-ttu-id="c3d19-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-176">The developer of the app.</span></span> <span data-ttu-id="c3d19-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-178">notes</span><span class="sxs-lookup"><span data-stu-id="c3d19-178">notes</span></span>|<span data-ttu-id="c3d19-179">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-179">String</span></span>|<span data-ttu-id="c3d19-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="c3d19-180">Notes for the app.</span></span> <span data-ttu-id="c3d19-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3d19-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="c3d19-182">publishingState</span></span>|[<span data-ttu-id="c3d19-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="c3d19-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c3d19-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-184">The publishing state for the app.</span></span> <span data-ttu-id="c3d19-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c3d19-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c3d19-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c3d19-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c3d19-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c3d19-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c3d19-188">committedContentVersion</span></span>|<span data-ttu-id="c3d19-189">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-189">String</span></span>|<span data-ttu-id="c3d19-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="c3d19-190">The internal committed content version.</span></span> <span data-ttu-id="c3d19-191">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c3d19-192">fileName</span><span class="sxs-lookup"><span data-stu-id="c3d19-192">fileName</span></span>|<span data-ttu-id="c3d19-193">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-193">String</span></span>|<span data-ttu-id="c3d19-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-194">The name of the main Lob application file.</span></span> <span data-ttu-id="c3d19-195">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c3d19-196">size</span><span class="sxs-lookup"><span data-stu-id="c3d19-196">size</span></span>|<span data-ttu-id="c3d19-197">Int64</span><span class="sxs-lookup"><span data-stu-id="c3d19-197">Int64</span></span>|<span data-ttu-id="c3d19-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="c3d19-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="c3d19-199">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3d19-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c3d19-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="c3d19-200">bundleId</span></span>|<span data-ttu-id="c3d19-201">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-201">String</span></span>|<span data-ttu-id="c3d19-202">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c3d19-202">The Identity Name.</span></span>|
|<span data-ttu-id="c3d19-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="c3d19-203">applicableDeviceType</span></span>|[<span data-ttu-id="c3d19-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c3d19-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="c3d19-205">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="c3d19-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="c3d19-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c3d19-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c3d19-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c3d19-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="c3d19-208">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c3d19-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c3d19-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c3d19-209">expirationDateTime</span></span>|<span data-ttu-id="c3d19-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3d19-210">DateTimeOffset</span></span>|<span data-ttu-id="c3d19-211">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="c3d19-211">The expiration time.</span></span>|
|<span data-ttu-id="c3d19-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="c3d19-212">versionNumber</span></span>|<span data-ttu-id="c3d19-213">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-213">String</span></span>|<span data-ttu-id="c3d19-214">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="c3d19-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c3d19-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="c3d19-215">buildNumber</span></span>|<span data-ttu-id="c3d19-216">String</span><span class="sxs-lookup"><span data-stu-id="c3d19-216">String</span></span>|<span data-ttu-id="c3d19-217">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="c3d19-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="c3d19-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3d19-218">Response</span></span>
<span data-ttu-id="c3d19-219">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3d19-219">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3d19-220">Пример</span><span class="sxs-lookup"><span data-stu-id="c3d19-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3d19-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d19-221">Request</span></span>
<span data-ttu-id="c3d19-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3d19-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="c3d19-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d19-223">Response</span></span>
<span data-ttu-id="c3d19-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3d19-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



