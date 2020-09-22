---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72cc707aea4fb9c85ef8e9aae3914f4da69e4ab3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063487"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="f7340-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="f7340-103">Update windowsMobileMSI</span></span>

<span data-ttu-id="f7340-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7340-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7340-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7340-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7340-106">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7340-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f7340-107">Prerequisites</span></span>
<span data-ttu-id="f7340-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7340-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7340-110">Permission type</span></span>|<span data-ttu-id="f7340-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7340-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7340-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7340-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7340-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7340-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7340-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7340-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7340-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7340-115">Not supported.</span></span>|
|<span data-ttu-id="f7340-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7340-116">Application</span></span>|<span data-ttu-id="f7340-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7340-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7340-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7340-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f7340-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7340-119">Request headers</span></span>
|<span data-ttu-id="f7340-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7340-120">Header</span></span>|<span data-ttu-id="f7340-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f7340-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7340-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7340-122">Authorization</span></span>|<span data-ttu-id="f7340-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7340-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7340-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f7340-124">Accept</span></span>|<span data-ttu-id="f7340-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7340-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7340-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7340-126">Request body</span></span>
<span data-ttu-id="f7340-127">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7340-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="f7340-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="f7340-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7340-129">Property</span></span>|<span data-ttu-id="f7340-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f7340-130">Type</span></span>|<span data-ttu-id="f7340-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f7340-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7340-132">id</span><span class="sxs-lookup"><span data-stu-id="f7340-132">id</span></span>|<span data-ttu-id="f7340-133">String</span><span class="sxs-lookup"><span data-stu-id="f7340-133">String</span></span>|<span data-ttu-id="f7340-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7340-134">Key of the entity.</span></span> <span data-ttu-id="f7340-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f7340-136">displayName</span></span>|<span data-ttu-id="f7340-137">String</span><span class="sxs-lookup"><span data-stu-id="f7340-137">String</span></span>|<span data-ttu-id="f7340-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f7340-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f7340-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-140">description</span><span class="sxs-lookup"><span data-stu-id="f7340-140">description</span></span>|<span data-ttu-id="f7340-141">String</span><span class="sxs-lookup"><span data-stu-id="f7340-141">String</span></span>|<span data-ttu-id="f7340-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-142">The description of the app.</span></span> <span data-ttu-id="f7340-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f7340-144">publisher</span></span>|<span data-ttu-id="f7340-145">String</span><span class="sxs-lookup"><span data-stu-id="f7340-145">String</span></span>|<span data-ttu-id="f7340-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-146">The publisher of the app.</span></span> <span data-ttu-id="f7340-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f7340-148">largeIcon</span></span>|[<span data-ttu-id="f7340-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f7340-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f7340-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f7340-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f7340-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7340-152">createdDateTime</span></span>|<span data-ttu-id="f7340-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7340-153">DateTimeOffset</span></span>|<span data-ttu-id="f7340-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-154">The date and time the app was created.</span></span> <span data-ttu-id="f7340-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7340-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f7340-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7340-157">DateTimeOffset</span></span>|<span data-ttu-id="f7340-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f7340-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f7340-160">isFeatured</span></span>|<span data-ttu-id="f7340-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7340-161">Boolean</span></span>|<span data-ttu-id="f7340-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f7340-163">privacyInformationUrl</span></span>|<span data-ttu-id="f7340-164">String</span><span class="sxs-lookup"><span data-stu-id="f7340-164">String</span></span>|<span data-ttu-id="f7340-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f7340-165">The privacy statement Url.</span></span> <span data-ttu-id="f7340-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f7340-167">informationUrl</span></span>|<span data-ttu-id="f7340-168">String</span><span class="sxs-lookup"><span data-stu-id="f7340-168">String</span></span>|<span data-ttu-id="f7340-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f7340-169">The more information Url.</span></span> <span data-ttu-id="f7340-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-171">owner</span><span class="sxs-lookup"><span data-stu-id="f7340-171">owner</span></span>|<span data-ttu-id="f7340-172">String</span><span class="sxs-lookup"><span data-stu-id="f7340-172">String</span></span>|<span data-ttu-id="f7340-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-173">The owner of the app.</span></span> <span data-ttu-id="f7340-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-175">developer</span><span class="sxs-lookup"><span data-stu-id="f7340-175">developer</span></span>|<span data-ttu-id="f7340-176">String</span><span class="sxs-lookup"><span data-stu-id="f7340-176">String</span></span>|<span data-ttu-id="f7340-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-177">The developer of the app.</span></span> <span data-ttu-id="f7340-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-179">notes</span><span class="sxs-lookup"><span data-stu-id="f7340-179">notes</span></span>|<span data-ttu-id="f7340-180">String</span><span class="sxs-lookup"><span data-stu-id="f7340-180">String</span></span>|<span data-ttu-id="f7340-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-181">Notes for the app.</span></span> <span data-ttu-id="f7340-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7340-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="f7340-183">publishingState</span></span>|[<span data-ttu-id="f7340-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f7340-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f7340-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-185">The publishing state for the app.</span></span> <span data-ttu-id="f7340-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f7340-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f7340-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f7340-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f7340-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f7340-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f7340-189">committedContentVersion</span></span>|<span data-ttu-id="f7340-190">String</span><span class="sxs-lookup"><span data-stu-id="f7340-190">String</span></span>|<span data-ttu-id="f7340-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="f7340-191">The internal committed content version.</span></span> <span data-ttu-id="f7340-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f7340-193">fileName</span><span class="sxs-lookup"><span data-stu-id="f7340-193">fileName</span></span>|<span data-ttu-id="f7340-194">String</span><span class="sxs-lookup"><span data-stu-id="f7340-194">String</span></span>|<span data-ttu-id="f7340-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f7340-195">The name of the main Lob application file.</span></span> <span data-ttu-id="f7340-196">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f7340-197">size</span><span class="sxs-lookup"><span data-stu-id="f7340-197">size</span></span>|<span data-ttu-id="f7340-198">Int64</span><span class="sxs-lookup"><span data-stu-id="f7340-198">Int64</span></span>|<span data-ttu-id="f7340-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="f7340-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="f7340-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7340-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f7340-201">commandLine</span><span class="sxs-lookup"><span data-stu-id="f7340-201">commandLine</span></span>|<span data-ttu-id="f7340-202">String</span><span class="sxs-lookup"><span data-stu-id="f7340-202">String</span></span>|<span data-ttu-id="f7340-203">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="f7340-203">The command line.</span></span>|
|<span data-ttu-id="f7340-204">productCode</span><span class="sxs-lookup"><span data-stu-id="f7340-204">productCode</span></span>|<span data-ttu-id="f7340-205">String</span><span class="sxs-lookup"><span data-stu-id="f7340-205">String</span></span>|<span data-ttu-id="f7340-206">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="f7340-206">The product code.</span></span>|
|<span data-ttu-id="f7340-207">productVersion</span><span class="sxs-lookup"><span data-stu-id="f7340-207">productVersion</span></span>|<span data-ttu-id="f7340-208">String</span><span class="sxs-lookup"><span data-stu-id="f7340-208">String</span></span>|<span data-ttu-id="f7340-209">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="f7340-209">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f7340-210">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="f7340-210">ignoreVersionDetection</span></span>|<span data-ttu-id="f7340-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7340-211">Boolean</span></span>|<span data-ttu-id="f7340-212">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="f7340-212">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="f7340-213">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="f7340-213">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="f7340-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7340-214">Response</span></span>
<span data-ttu-id="f7340-215">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7340-215">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7340-216">Пример</span><span class="sxs-lookup"><span data-stu-id="f7340-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7340-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7340-217">Request</span></span>
<span data-ttu-id="f7340-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7340-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="f7340-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7340-219">Response</span></span>
<span data-ttu-id="f7340-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7340-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```









