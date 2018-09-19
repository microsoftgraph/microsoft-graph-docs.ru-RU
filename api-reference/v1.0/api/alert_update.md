# <a name="update-alert"></a>Оповещение обновления

Обновите редактируемое свойство **оповещения** в любом интегрированном решении для синхронизации состояний оповещений и назначений в синхронизации решений. Этот метод обновляет все решения, у которых есть запись идентификатора указанного оповещения.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

> **Примечание:** с этим методом необходимо указать идентификатор **оповещения** в качестве параметра и информацию о производителе, содержащую `provider` и `vendor`.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | "Bearer {код}". Обязательный.|
|Prefer | return=representation |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите представление JSON для соответствующих полей, которые необходимо обновить. Текст **должен** содержать `vendorInformation` свойство с допустимыми полями `provider` и `vendor`. В следующей таблице приведены поля, которые могут быть обновлены для оповещения. Значения для существующих свойств, которые не включены в текст запроса, остаются без изменений. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|assignedTo|String|Имя аналитики, которой назначено оповещение для рассмотрения, исследования и исправления.|
|closedDateTime|DateTimeOffset|Дата и время закрытия оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение для полуночи 1 января 2014 года в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|comments|Коллекция String|Комментарии аналитика по оповещению (для управления предупреждениями клиента).|
|feedback|alertFeedback|Отчет аналитика относительно оповещения. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|alertStatus|Статус жизненного цикла оповещения (стадия). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|Коллекция String|Определяемые пользователем метки, которые могут применяться к оповещению и выступать в качестве условий фильтра (например, "HVA", "SAW").|
|vendorInformation *|[securityVendorInformation](../resources/securityvendorinformation.md)|Комплексный тип, в котором содержатся сведения о безопасности продуктов и услуг разработчика, поставщика и субпоставщика (например, производитель = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker). **Поля поставщика и производителя являются обязательными.**|
(\* Указывает на обязательное поле.)

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется запрос на необязательный заголовок, метод возвращает код отклика `200 OK` и обновленный объект [оповещения](../resources/alert.md) в теле ответа.

## <a name="example-1"></a>Пример 1

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>Отклик

Ниже приведен пример успешного отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>Пример 2

### <a name="request"></a>Запрос

В следующем примере показан запрос, который включает в себя заголовок запроса `Prefer`.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика, в котором используется необязательный заголовок запроса `Prefer: return=representation`.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
