---
title: Создание win32LobApp
description: Создание нового объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c903de1e1f2bec92c255d29878eac06d38f4428c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080099"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="b13cd-103">Создание win32LobApp</span><span class="sxs-lookup"><span data-stu-id="b13cd-103">Create win32LobApp</span></span>

<span data-ttu-id="b13cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b13cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b13cd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b13cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b13cd-106">Создание нового объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b13cd-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b13cd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b13cd-107">Prerequisites</span></span>
<span data-ttu-id="b13cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b13cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b13cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b13cd-110">Permission type</span></span>|<span data-ttu-id="b13cd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b13cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b13cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b13cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b13cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b13cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b13cd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b13cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b13cd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13cd-115">Not supported.</span></span>|
|<span data-ttu-id="b13cd-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b13cd-116">Application</span></span>|<span data-ttu-id="b13cd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b13cd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b13cd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b13cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b13cd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b13cd-119">Request headers</span></span>
|<span data-ttu-id="b13cd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b13cd-120">Header</span></span>|<span data-ttu-id="b13cd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b13cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b13cd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b13cd-122">Authorization</span></span>|<span data-ttu-id="b13cd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b13cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b13cd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b13cd-124">Accept</span></span>|<span data-ttu-id="b13cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b13cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b13cd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b13cd-126">Request body</span></span>
<span data-ttu-id="b13cd-127">В тексте запроса добавьте представление объекта win32LobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b13cd-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="b13cd-128">В следующей таблице приведены свойства, необходимые при создании win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="b13cd-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="b13cd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b13cd-129">Property</span></span>|<span data-ttu-id="b13cd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b13cd-130">Type</span></span>|<span data-ttu-id="b13cd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b13cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b13cd-132">id</span><span class="sxs-lookup"><span data-stu-id="b13cd-132">id</span></span>|<span data-ttu-id="b13cd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-133">String</span></span>|<span data-ttu-id="b13cd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b13cd-134">Key of the entity.</span></span> <span data-ttu-id="b13cd-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b13cd-136">displayName</span></span>|<span data-ttu-id="b13cd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-137">String</span></span>|<span data-ttu-id="b13cd-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b13cd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b13cd-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-140">description</span><span class="sxs-lookup"><span data-stu-id="b13cd-140">description</span></span>|<span data-ttu-id="b13cd-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-141">String</span></span>|<span data-ttu-id="b13cd-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-142">The description of the app.</span></span> <span data-ttu-id="b13cd-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b13cd-144">publisher</span></span>|<span data-ttu-id="b13cd-145">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-145">String</span></span>|<span data-ttu-id="b13cd-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-146">The publisher of the app.</span></span> <span data-ttu-id="b13cd-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b13cd-148">largeIcon</span></span>|[<span data-ttu-id="b13cd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b13cd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b13cd-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b13cd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b13cd-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b13cd-152">createdDateTime</span></span>|<span data-ttu-id="b13cd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b13cd-153">DateTimeOffset</span></span>|<span data-ttu-id="b13cd-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-154">The date and time the app was created.</span></span> <span data-ttu-id="b13cd-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b13cd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b13cd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b13cd-157">DateTimeOffset</span></span>|<span data-ttu-id="b13cd-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b13cd-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b13cd-160">isFeatured</span></span>|<span data-ttu-id="b13cd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b13cd-161">Boolean</span></span>|<span data-ttu-id="b13cd-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b13cd-163">privacyInformationUrl</span></span>|<span data-ttu-id="b13cd-164">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-164">String</span></span>|<span data-ttu-id="b13cd-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b13cd-165">The privacy statement Url.</span></span> <span data-ttu-id="b13cd-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b13cd-167">informationUrl</span></span>|<span data-ttu-id="b13cd-168">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-168">String</span></span>|<span data-ttu-id="b13cd-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b13cd-169">The more information Url.</span></span> <span data-ttu-id="b13cd-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-171">owner</span><span class="sxs-lookup"><span data-stu-id="b13cd-171">owner</span></span>|<span data-ttu-id="b13cd-172">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-172">String</span></span>|<span data-ttu-id="b13cd-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-173">The owner of the app.</span></span> <span data-ttu-id="b13cd-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-175">developer</span><span class="sxs-lookup"><span data-stu-id="b13cd-175">developer</span></span>|<span data-ttu-id="b13cd-176">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-176">String</span></span>|<span data-ttu-id="b13cd-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-177">The developer of the app.</span></span> <span data-ttu-id="b13cd-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-179">notes</span><span class="sxs-lookup"><span data-stu-id="b13cd-179">notes</span></span>|<span data-ttu-id="b13cd-180">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-180">String</span></span>|<span data-ttu-id="b13cd-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-181">Notes for the app.</span></span> <span data-ttu-id="b13cd-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b13cd-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="b13cd-183">publishingState</span></span>|[<span data-ttu-id="b13cd-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b13cd-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b13cd-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-185">The publishing state for the app.</span></span> <span data-ttu-id="b13cd-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b13cd-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b13cd-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b13cd-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b13cd-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b13cd-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b13cd-189">committedContentVersion</span></span>|<span data-ttu-id="b13cd-190">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-190">String</span></span>|<span data-ttu-id="b13cd-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="b13cd-191">The internal committed content version.</span></span> <span data-ttu-id="b13cd-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b13cd-193">fileName</span><span class="sxs-lookup"><span data-stu-id="b13cd-193">fileName</span></span>|<span data-ttu-id="b13cd-194">String</span><span class="sxs-lookup"><span data-stu-id="b13cd-194">String</span></span>|<span data-ttu-id="b13cd-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-195">The name of the main Lob application file.</span></span> <span data-ttu-id="b13cd-196">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b13cd-197">size</span><span class="sxs-lookup"><span data-stu-id="b13cd-197">size</span></span>|<span data-ttu-id="b13cd-198">Int64</span><span class="sxs-lookup"><span data-stu-id="b13cd-198">Int64</span></span>|<span data-ttu-id="b13cd-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="b13cd-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="b13cd-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b13cd-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b13cd-201">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="b13cd-201">installCommandLine</span></span>|<span data-ttu-id="b13cd-202">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-202">String</span></span>|<span data-ttu-id="b13cd-203">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="b13cd-203">The command line to install this app</span></span>|
|<span data-ttu-id="b13cd-204">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="b13cd-204">uninstallCommandLine</span></span>|<span data-ttu-id="b13cd-205">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-205">String</span></span>|<span data-ttu-id="b13cd-206">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="b13cd-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="b13cd-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b13cd-207">applicableArchitectures</span></span>|[<span data-ttu-id="b13cd-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b13cd-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b13cd-209">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="b13cd-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b13cd-210">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="b13cd-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="b13cd-211">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="b13cd-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="b13cd-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b13cd-212">Int32</span></span>|<span data-ttu-id="b13cd-213">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="b13cd-214">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="b13cd-214">minimumMemoryInMB</span></span>|<span data-ttu-id="b13cd-215">Int32</span><span class="sxs-lookup"><span data-stu-id="b13cd-215">Int32</span></span>|<span data-ttu-id="b13cd-216">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="b13cd-217">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="b13cd-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="b13cd-218">Int32</span><span class="sxs-lookup"><span data-stu-id="b13cd-218">Int32</span></span>|<span data-ttu-id="b13cd-219">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="b13cd-220">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="b13cd-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="b13cd-221">Int32</span><span class="sxs-lookup"><span data-stu-id="b13cd-221">Int32</span></span>|<span data-ttu-id="b13cd-222">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="b13cd-223">правила</span><span class="sxs-lookup"><span data-stu-id="b13cd-223">rules</span></span>|<span data-ttu-id="b13cd-224">Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="b13cd-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="b13cd-225">Правила обнаружения и требований для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="b13cd-226">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="b13cd-226">installExperience</span></span>|[<span data-ttu-id="b13cd-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="b13cd-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="b13cd-228">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="b13cd-228">The install experience for this app.</span></span>|
|<span data-ttu-id="b13cd-229">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="b13cd-229">returnCodes</span></span>|<span data-ttu-id="b13cd-230">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="b13cd-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="b13cd-231">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="b13cd-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="b13cd-232">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="b13cd-232">msiInformation</span></span>|[<span data-ttu-id="b13cd-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="b13cd-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="b13cd-234">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="b13cd-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="b13cd-235">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="b13cd-235">setupFilePath</span></span>|<span data-ttu-id="b13cd-236">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-236">String</span></span>|<span data-ttu-id="b13cd-237">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="b13cd-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="b13cd-238">минимумсуппортедвиндовсрелеасе</span><span class="sxs-lookup"><span data-stu-id="b13cd-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="b13cd-239">Строка</span><span class="sxs-lookup"><span data-stu-id="b13cd-239">String</span></span>|<span data-ttu-id="b13cd-240">Значение минимального поддерживаемого выпуска Windows.</span><span class="sxs-lookup"><span data-stu-id="b13cd-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="b13cd-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="b13cd-241">Response</span></span>
<span data-ttu-id="b13cd-242">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b13cd-242">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b13cd-243">Пример</span><span class="sxs-lookup"><span data-stu-id="b13cd-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="b13cd-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="b13cd-244">Request</span></span>
<span data-ttu-id="b13cd-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b13cd-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2134

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="b13cd-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="b13cd-246">Response</span></span>
<span data-ttu-id="b13cd-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b13cd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2306

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```






