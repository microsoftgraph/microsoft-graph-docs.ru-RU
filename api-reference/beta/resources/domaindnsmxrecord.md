<a id="domaindnsmxrecord-resource-type" class="xliff"></a>
# Тип ресурса domainDnsMxRecord

Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).

<a id="methods" class="xliff"></a>
## Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).

<a id="properties" class="xliff"></a>
## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.|
|isOptional|Boolean| Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись MX на узле DNS. |
|label|String| Значение, используемое при настройке свойства *псевдонима, узла или имени* для записи MX на узле DNS. |
|mailExchange|String| Значение, используемое при настройке *значения, ответа или целевого объекта* для записи MX на узле DNS.|
|preference|Int32| Значение, используемое при настройке свойства *приоритета или предпочтения* для записи MX на узле DNS. |
|recordType|String| Тип записи DNS. Это свойство всегда имеет значение *Mx*. Ключ. |
|supportedService|String| Служба или компонент Microsoft Online Services, зависящие от этой записи типа MX.</br></br>Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*. |
|ttl|Int32| Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null. |

<a id="relationships" class="xliff"></a>
## Связи
Нет

<a id="json-representation" class="xliff"></a>
## Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->