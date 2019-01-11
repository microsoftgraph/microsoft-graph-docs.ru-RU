---
title: Create windowsMobileMSI
description: Создание объекта windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 868bfa82b8f7b5de70a56d681b8a0a48eee59ec4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878108"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="a701d-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="a701d-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="a701d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a701d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a701d-105">Создание объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-105">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a701d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a701d-106">Prerequisites</span></span>
<span data-ttu-id="a701d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a701d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a701d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a701d-109">Permission type</span></span>|<span data-ttu-id="a701d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a701d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a701d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a701d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a701d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a701d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a701d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a701d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a701d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a701d-114">Not supported.</span></span>|
|<span data-ttu-id="a701d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a701d-115">Application</span></span>|<span data-ttu-id="a701d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a701d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a701d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a701d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a701d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a701d-118">Request headers</span></span>
|<span data-ttu-id="a701d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a701d-119">Header</span></span>|<span data-ttu-id="a701d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a701d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a701d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a701d-121">Authorization</span></span>|<span data-ttu-id="a701d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a701d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a701d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a701d-123">Accept</span></span>|<span data-ttu-id="a701d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a701d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a701d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a701d-125">Request body</span></span>
<span data-ttu-id="a701d-126">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a701d-126">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="a701d-127">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="a701d-127">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="a701d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a701d-128">Property</span></span>|<span data-ttu-id="a701d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a701d-129">Type</span></span>|<span data-ttu-id="a701d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a701d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a701d-131">id</span><span class="sxs-lookup"><span data-stu-id="a701d-131">id</span></span>|<span data-ttu-id="a701d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a701d-132">String</span></span>|<span data-ttu-id="a701d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a701d-133">Key of the entity.</span></span> <span data-ttu-id="a701d-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a701d-135">displayName</span></span>|<span data-ttu-id="a701d-136">String</span><span class="sxs-lookup"><span data-stu-id="a701d-136">String</span></span>|<span data-ttu-id="a701d-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a701d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a701d-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-139">описание</span><span class="sxs-lookup"><span data-stu-id="a701d-139">description</span></span>|<span data-ttu-id="a701d-140">String</span><span class="sxs-lookup"><span data-stu-id="a701d-140">String</span></span>|<span data-ttu-id="a701d-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-141">The description of the app.</span></span> <span data-ttu-id="a701d-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a701d-143">publisher</span></span>|<span data-ttu-id="a701d-144">String</span><span class="sxs-lookup"><span data-stu-id="a701d-144">String</span></span>|<span data-ttu-id="a701d-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-145">The publisher of the app.</span></span> <span data-ttu-id="a701d-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a701d-147">largeIcon</span></span>|[<span data-ttu-id="a701d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a701d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a701d-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a701d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a701d-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a701d-151">createdDateTime</span></span>|<span data-ttu-id="a701d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a701d-152">DateTimeOffset</span></span>|<span data-ttu-id="a701d-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-153">The date and time the app was created.</span></span> <span data-ttu-id="a701d-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a701d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a701d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a701d-156">DateTimeOffset</span></span>|<span data-ttu-id="a701d-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="a701d-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a701d-159">isFeatured</span></span>|<span data-ttu-id="a701d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a701d-160">Boolean</span></span>|<span data-ttu-id="a701d-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a701d-162">privacyInformationUrl</span></span>|<span data-ttu-id="a701d-163">String</span><span class="sxs-lookup"><span data-stu-id="a701d-163">String</span></span>|<span data-ttu-id="a701d-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a701d-164">The privacy statement Url.</span></span> <span data-ttu-id="a701d-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a701d-166">informationUrl</span></span>|<span data-ttu-id="a701d-167">String</span><span class="sxs-lookup"><span data-stu-id="a701d-167">String</span></span>|<span data-ttu-id="a701d-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a701d-168">The more information Url.</span></span> <span data-ttu-id="a701d-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-170">owner</span><span class="sxs-lookup"><span data-stu-id="a701d-170">owner</span></span>|<span data-ttu-id="a701d-171">String</span><span class="sxs-lookup"><span data-stu-id="a701d-171">String</span></span>|<span data-ttu-id="a701d-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-172">The owner of the app.</span></span> <span data-ttu-id="a701d-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-174">developer</span><span class="sxs-lookup"><span data-stu-id="a701d-174">developer</span></span>|<span data-ttu-id="a701d-175">String</span><span class="sxs-lookup"><span data-stu-id="a701d-175">String</span></span>|<span data-ttu-id="a701d-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-176">The developer of the app.</span></span> <span data-ttu-id="a701d-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-178">notes</span><span class="sxs-lookup"><span data-stu-id="a701d-178">notes</span></span>|<span data-ttu-id="a701d-179">String</span><span class="sxs-lookup"><span data-stu-id="a701d-179">String</span></span>|<span data-ttu-id="a701d-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a701d-180">Notes for the app.</span></span> <span data-ttu-id="a701d-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a701d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="a701d-182">publishingState</span></span>|[<span data-ttu-id="a701d-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a701d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a701d-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-184">The publishing state for the app.</span></span> <span data-ttu-id="a701d-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a701d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a701d-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a701d-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a701d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a701d-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a701d-188">committedContentVersion</span></span>|<span data-ttu-id="a701d-189">String</span><span class="sxs-lookup"><span data-stu-id="a701d-189">String</span></span>|<span data-ttu-id="a701d-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="a701d-190">The internal committed content version.</span></span> <span data-ttu-id="a701d-191">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a701d-192">fileName</span><span class="sxs-lookup"><span data-stu-id="a701d-192">fileName</span></span>|<span data-ttu-id="a701d-193">String</span><span class="sxs-lookup"><span data-stu-id="a701d-193">String</span></span>|<span data-ttu-id="a701d-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="a701d-194">The name of the main Lob application file.</span></span> <span data-ttu-id="a701d-195">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a701d-196">size</span><span class="sxs-lookup"><span data-stu-id="a701d-196">size</span></span>|<span data-ttu-id="a701d-197">Int64</span><span class="sxs-lookup"><span data-stu-id="a701d-197">Int64</span></span>|<span data-ttu-id="a701d-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="a701d-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="a701d-199">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a701d-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a701d-200">commandLine</span><span class="sxs-lookup"><span data-stu-id="a701d-200">commandLine</span></span>|<span data-ttu-id="a701d-201">String</span><span class="sxs-lookup"><span data-stu-id="a701d-201">String</span></span>|<span data-ttu-id="a701d-202">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="a701d-202">The command line.</span></span>|
|<span data-ttu-id="a701d-203">productCode</span><span class="sxs-lookup"><span data-stu-id="a701d-203">productCode</span></span>|<span data-ttu-id="a701d-204">String</span><span class="sxs-lookup"><span data-stu-id="a701d-204">String</span></span>|<span data-ttu-id="a701d-205">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="a701d-205">The product code.</span></span>|
|<span data-ttu-id="a701d-206">productVersion</span><span class="sxs-lookup"><span data-stu-id="a701d-206">productVersion</span></span>|<span data-ttu-id="a701d-207">String</span><span class="sxs-lookup"><span data-stu-id="a701d-207">String</span></span>|<span data-ttu-id="a701d-208">Версия бизнес-приложения MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="a701d-208">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a701d-209">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="a701d-209">ignoreVersionDetection</span></span>|<span data-ttu-id="a701d-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a701d-210">Boolean</span></span>|<span data-ttu-id="a701d-211">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a701d-211">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="a701d-212">Для бизнес-приложений MSI Windows Mobile с функцией самостоятельного обновления следует использовать значение true.</span><span class="sxs-lookup"><span data-stu-id="a701d-212">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="a701d-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="a701d-213">Response</span></span>
<span data-ttu-id="a701d-214">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a701d-214">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a701d-215">Пример</span><span class="sxs-lookup"><span data-stu-id="a701d-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="a701d-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="a701d-216">Request</span></span>
<span data-ttu-id="a701d-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a701d-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="a701d-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="a701d-218">Response</span></span>
<span data-ttu-id="a701d-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a701d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



